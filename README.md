<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>RB! AI v1.0 (FREE)</title>
  <style>
    body { font-family: Arial; background:#111; color:#eee; }
    #chat { max-width:600px; margin:auto; padding:20px; }
    input, button {
      width:100%; padding:10px; margin-top:5px;
      background:#222; color:#eee; border:1px solid #444;
      box-sizing:border-box;
    }
    #output { margin-top:15px; min-height:100px; white-space:pre-line; }
  </style>
</head>
<body>
  <div id="chat">
    <h2>RB! AI v1.0 (FREE)</h2>
    <input id="userInput" placeholder="Ask me something..." />
    <button onclick="reply()">Send</button>
    <div id="output"></div>
  </div>

<script>
function reply() {
  const input = document.getElementById("userInput").value.toLowerCase();
  let response = "I can't answer that clearly right now. I need more lore.";

  // Simple keyword-based responses
  if (input.includes("undertale")) {
    response = "Undertale Real Breath gives a darker and more dramatic perspective on the classic Undertale universe.";
  } 
  if (input.includes("under!prime")) {
    response = "Under!Prime focuses on the conflict between parallel universes and has a more aggressive storyline.";
  } 
  if (input.includes("rb")) {
    response = "RB! is the creator of these universes. The storytelling is harsh yet emotional.";
  } 
  if (input.includes("story") || input.includes("scene")) {
    response = "I suggest a scene that highlights the inner conflicts of the characters.";
  }

  document.getElementById("output").innerText = response;
}
</script>
</body>
</html>
