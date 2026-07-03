let currentSentence = "";

function say(sentence) {
  currentSentence = sentence;
  document.getElementById("sentenceBox").innerText = sentence;
  speakSentence();
}

function clearSentence() {
  currentSentence = "";
  document.getElementById("sentenceBox").innerText = "اختاري زر";
}

function speakSentence() {
  if (!currentSentence) return;

  speechSynthesis.cancel();

  let textOnly = currentSentence.replace(/[^\u0600-\u06FF\s]/g, "");

  const speech = new SpeechSynthesisUtterance(textOnly);
  speech.lang = "ar-SA";
  speech.rate = 0.75;

  speechSynthesis.speak(speech);
}
