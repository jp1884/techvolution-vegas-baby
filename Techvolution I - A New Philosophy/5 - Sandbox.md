
<!-- Forward JS Language Test Code May 14 2023 -->
<script setup>
  // button Variables
  import { ref } from 'vue'
  let languageBlank=ref(false)
  let languageSpanish=ref(false)
  let languageEnglish=ref(false)

  // color and word variables
  const wordsBlank = ["########"];
  const wordsSpanish = ["Azul", "Verde", "Amarillo", "Negro", "Blanco", "Rojo", "Gris", "Rosado", "Marrón", "Plata"];
  const wordsEnglish = ["Maroon","Red","Orange","Yellow","Green","Purple","Pink","Lime","Teal","Aqua","Blue","Black","Gray","Silver", "White"];
  const colors = ["Maroon","Red","Orange","Yellow","Green","Purple","Pink","Lime","Teal","Aqua","Blue","Gray","Silver"];

// Note:
// To have another language requires a set of new functions, for example "wordsSpanish" replaced by "wordsEnglish"
// This version doesn't use an if/else statement. If needed, see other Language Test version that integrates several languages into one set of functions.
// This code could be simplified but is good enough for now.

// Blank Function
// Function reaches out and grabs "Blank/Spanish/English" words and colors from the arrays. 
// I removed the Spanish test, but it could be re-added by duplicating this code and inputting Spanish over English
function selectWordAndColorBlank() {
  let wordBlank = document.getElementById("wordBlank");
  let wordBlankIndex = Math.floor(Math.random() * wordsBlank.length);
  let randomWord = wordsBlank[wordBlankIndex];
  let colorIndex = Math.floor(Math.random() * colors.length);
  let randomColor = colors[colorIndex];
  wordBlank.innerText = randomWord;
  wordBlank.style.color = randomColor;
}

// function that grabs and displays chosen words in timed intervals
function startTestBlank() {
  languageBlank.value = false
  languageBlank.value = true
  languageEnglish.value = false
    let counter = 0;
    let intervalId = setInterval(selectWordAndColorBlank, 700);
    setTimeout(function() {
        clearInterval(intervalId);
    counter = 0;
      setTimeout(function() {
      languageBlank.value = false; languageEnglish.value = false; languageBlank.value = false;   }, 700)
  }, 10000);
}

// English Function. Same as "Blank" functions but chosing "English" words
function selectWordAndColorEnglish() {
  let wordEnglish = document.getElementById("wordEnglish");
  let wordEnglishIndex = Math.floor(Math.random() * wordsEnglish.length);
  let randomWord = wordsEnglish[wordEnglishIndex];
  let colorIndex = Math.floor(Math.random() * colors.length);
  let randomColor = colors[colorIndex];
  wordEnglish.innerText = randomWord;
  wordEnglish.style.color = randomColor;
}

function startTestEnglish() {
  languageBlank.value = false
  languageSpanish.value = false
  languageEnglish.value = true
  let counter = 0;
  let intervalId = setInterval(selectWordAndColorEnglish, 700);
  setTimeout(function() {
    clearInterval(intervalId);
    counter = 0;
    setTimeout(function() {
    languageBlank.value = false; languageEnglish.value = false; languageSpanish.value = false;  }, 700)
  }, 10000);
}

</script>

<style>
  /* Language Test CSS code*/
/* toggle button */
.t-btn {
  background-color: blueviolet !important;
  font-size: 18px !important;
  border-radius: 5px !important;
  padding: 4px 20px !important;
  margin: 10px 20px 10px 0px !important;
}

.t-btn-disabled {
  background-color: rgb(184, 128, 236) !important;
  font-size: 18px !important;
  border-radius: 5px !important;
  padding: 4px 20px !important;
  margin: 10px 20px 10px 0px !important;
}

.language-test{
  margin: 0px 0px !important;
  background-color: #00000000 !important;
  min-height: 40px !important;
}

.language-test p {
  margin: 0px 0px !important;
  font-size: 26px !important;
  font-Weight: bold !important;
  background-color: #00000000 !important;
}

</style>

<!-- Language Test HTML Buttons code and Display area -->
<button class="t-btn" v-if="!languageBlank" @click="startTestBlank()">Blank</button>
<button class="t-btn-disabled" v-if="languageBlank" disabled>...</button>
<button class="t-btn" v-if="!languageEnglish" @click="startTestEnglish()">English</button> 
<button class="t-btn-disabled" v-if="languageEnglish" disabled>...</button>

<div class="language-test">
  <p v-if="languageBlank" id="wordBlank"></p>
  <p v-if="languageEnglish" id="wordEnglish"></p>
</div>

