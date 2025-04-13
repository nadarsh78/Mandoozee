
<html lang="ml">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>🌸✨</title>
  <style>
    body {
      background-color: white;
      color: black;
      font-family: 'Segoe UI', sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      font-size: 1.5em;
      text-align: center;
      padding: 20px;
    }
    #text {
      transition: opacity 0.5s ease-in-out;
    }
  </style>
</head>
<body>
  <div id="text">പൂക്കളെ പോലും അഴക് പഠിപ്പിക്കുന്ന ആ ചിരിക്ക് വിഷുദിനാശംസകൾ!</div>

  <script>
    const messages = [
      "പൂക്കളെ പോലും അഴക് പഠിപ്പിക്കുന്ന ആ ചിരിക്ക് വിഷുദിനാശംസകൾ!",
      "🌸 Happy Vishu, my precious Ammukutty 🌸",
      "ഈ വിഷുവിൽ ഞാൻ അപേക്ഷിക്കുന്ന ഒരേൊരു കാര്യമുണ്ട് – നീ എന്നോട് എന്നും കൂടെയിരിക്കണം.",
      "😘💛"
    ];

    const duration = 6000; // 6 seconds per message
    let index = 1;
    const textElement = document.getElementById("text");

    function showNextMessage() {
      if (index < messages.length) {
        textElement.style.opacity = 0;
        setTimeout(() => {
          textElement.textContent = messages[index];
          textElement.style.opacity = 1;
          setTimeout(showNextMessage, duration);
          index++;
        }, 500);
      }
    }

    setTimeout(showNextMessage, duration);
  </script>
</body>
</html>
