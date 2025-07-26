
<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8">
  <title>Озвучення трьома мовами (Web Speech API)</title>
</head>
<body>
  <h2>🗣 Озвучення 5 речень трьома мовами</h2>
  <p>Натисніть кнопку, щоб почути озвучення українською, англійською або іспанською.</p>

  <p><strong>1. Я є лікар. / I am a doctor. / Yo soy médico.</strong><br>
    <button onclick="speak('Я є лікар.', 'uk-UA')">🇺🇦 Озвучити</button>
    <button onclick="speak('I am a doctor.', 'en-US')">🇬🇧 Speak</button>
    <button onclick="speak('Yo soy médico.', 'es-ES')">🇪🇸 Hablar</button>
  </p>

  <p><strong>2. Вона є добра. / She is kind. / Ella está feliz.</strong><br>
    <button onclick="speak('Вона є добра.', 'uk-UA')">🇺🇦 Озвучити</button>
    <button onclick="speak('She is kind.', 'en-US')">🇬🇧 Speak</button>
    <button onclick="speak('Ella está feliz.', 'es-ES')">🇪🇸 Hablar</button>
  </p>

  <p><strong>3. Ми є тут. / We are here. / Nosotros estamos aquí.</strong><br>
    <button onclick="speak('Ми є тут.', 'uk-UA')">🇺🇦 Озвучити</button>
    <button onclick="speak('We are here.', 'en-US')">🇬🇧 Speak</button>
    <button onclick="speak('Nosotros estamos aquí.', 'es-ES')">🇪🇸 Hablar</button>
  </p>

  <p><strong>4. Їх є троє. / There are three of them. / Son tres.</strong><br>
    <button onclick="speak('Їх є троє.', 'uk-UA')">🇺🇦 Озвучити</button>
    <button onclick="speak('There are three of them.', 'en-US')">🇬🇧 Speak</button>
    <button onclick="speak('Son tres.', 'es-ES')">🇪🇸 Hablar</button>
  </p>

  <p><strong>5. Це є вона. / This is her. / Esta es ella.</strong><br>
    <button onclick="speak('Це є вона.', 'uk-UA')">🇺🇦 Озвучити</button>
    <button onclick="speak('This is her.', 'en-US')">🇬🇧 Speak</button>
    <button onclick="speak('Esta es ella.', 'es-ES')">🇪🇸 Hablar</button>
  </p>

  <script>
    function speak(text, lang) {
      const utterance = new SpeechSynthesisUtterance(text);
      utterance.lang = lang;
      speechSynthesis.speak(utterance);
    }
  </script>
</body>
</html>
