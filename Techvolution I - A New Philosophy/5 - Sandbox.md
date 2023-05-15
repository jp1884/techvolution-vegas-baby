
<!-- Forward JS Language Test Code May 14 2023 -->

<script setup>
  // Button Variables
  import { ref } from 'vue'
  let languageBlank=ref(false)
  let languageSpanish=ref(false)
  let languageEnglish=ref(false)

  let counter = ref(0);

// Mainly JS Version
var wordsBlank = ["########"];
var wordsSpanish = ["Azul", "Verde", "Amarillo", "Negro", "Blanco", "Rojo", "Gris", "Rosado", "Marrón", "Plata"];
var wordsEnglish = ["Maroon","Red","Orange","Yellow","Olive","Green","Purple","Pink","Lime","Teal","Aqua","Blue","Navy","Black","Gray","Silver", "White"];
var colors = ["Maroon","Red","Orange","Yellow","Olive","Green","Purple","{Pink","Lime","Teal","Aqua","Blue","Navy","Gray","Silver"];

// Stop All

function stopAll() {
  languageBlank.value = false;
  languageSpanish.value = false;
  languageEnglish.value = false;
}

// Blank Function
function selectWordAndColorBlank() {
  var wordBlank = document.getElementById("wordBlank");
  var wordBlankIndex = Math.floor(Math.random() * wordsBlank.length);
  var randomWord = wordsBlank[wordBlankIndex];
  var colorIndex = Math.floor(Math.random() * colors.length);
  var randomColor = colors[colorIndex];
  wordBlank.innerText = randomWord;
  wordBlank.style.color = randomColor;
}

// simplified function, keeping around for reference if needed
// function changeWordAndColorBlank() {
//   setInterval(selectWordAndColorBlank, 1000);
// }

function changeWordAndColorBlank() {
  languageBlank.value = true
  languageSpanish.value = false
  languageEnglish.value = false
  // declare a counter variable and assign it to 0
  var counter = 0;
  // use setInterval to call selectWordAndColorEnglish every second and store the returned id in a variable
  var intervalId = setInterval(selectWordAndColorBlank, 700);
  // use setTimeout to call a function that clears the interval after 10 seconds
  setTimeout(function() {
    // use clearInterval to stop the interval using the id
    clearInterval(intervalId);
    // reset the counter to 0
    counter = 0;
    // delay final word for 700 ms
    setTimeout(function() {
    languageBlank.value = false; languageEnglish.value = false; languageSpanish.value = false;   }, 700)
  }, 10000); // 10000 milliseconds = 10 seconds
}

// Spanish Function
function selectWordAndColorSpanish() {
  var wordSpanish = document.getElementById("wordSpanish");
  var wordSpanishIndex = Math.floor(Math.random() * wordsSpanish.length);
  var randomWord = wordsSpanish[wordSpanishIndex];
  var colorIndex = Math.floor(Math.random() * colors.length);
  var randomColor = colors[colorIndex];
  wordSpanish.innerText = randomWord;
  wordSpanish.style.color = randomColor;
}

function changeWordAndColorSpanish() {
  languageBlank.value = false
  languageSpanish.value = true
  languageEnglish.value = false
    var counter = 0;
    var intervalId = setInterval(selectWordAndColorSpanish, 700);
    setTimeout(function() {
        clearInterval(intervalId);
    counter = 0;
      setTimeout(function() {
      languageBlank.value = false; languageEnglish.value = false; languageSpanish.value = false;   }, 700)
  }, 10000);
}

// English Function
function selectWordAndColorEnglish() {
  var wordEnglish = document.getElementById("wordEnglish");
  var wordEnglishIndex = Math.floor(Math.random() * wordsEnglish.length);
  var randomWord = wordsEnglish[wordEnglishIndex];
  var colorIndex = Math.floor(Math.random() * colors.length);
  var randomColor = colors[colorIndex];
  wordEnglish.innerText = randomWord;
  wordEnglish.style.color = randomColor;
}

function changeWordAndColorEnglish() {
  languageBlank.value = false
  languageSpanish.value = false
  languageEnglish.value = true
  var counter = 0;
  var intervalId = setInterval(selectWordAndColorEnglish, 700);
  setTimeout(function() {
    clearInterval(intervalId);
    counter = 0;
    setTimeout(function() {
    languageBlank.value = false; languageEnglish.value = false; languageSpanish.value = false;   }, 700)
  }, 10000);
}

</script>