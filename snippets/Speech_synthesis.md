### Speech synthesis

Currently The SpeechSynthesisUtterance interface of the Web Speech API represents a speech request. 
It contains the content the speech service should read and information about how to read it (e.g. language, pitch and volume.)

To know more - https://developer.mozilla.org/en-US/docs/Web/API/SpeechSynthesisUtterance

```
const speak = message => {
  const msg = new SpeechSynthesisUtterance(message);
  msg.voice = window.speechSynthesis.getVoices()[0];
  window.speechSynthesis.speak(msg);
}
speak('Hello, World')
```
