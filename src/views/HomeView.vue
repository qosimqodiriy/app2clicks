<script setup>
import { onMounted } from "vue";

var uagent = navigator.userAgent.toLowerCase();

function DetectIphone() {
  if (navigator.userAgent.match(/iPad/i)) {
    //code for iPad here
    console.log("Ipad");
    window.location.href = "https://apps.apple.com/uz/app/2clicks/id6444673015"

  } else if (navigator.userAgent.match(/iPhone/i)) {
    //code for iPhone here
    console.log("Iphone");
    window.location.href = "https://apps.apple.com/uz/app/2clicks/id6444673015"

  } else if (navigator.userAgent.match(/Android/i)) {
    //code for Android here
    console.log("Android");
    window.location.href = "https://play.google.com/store/apps/details?id=app.twoclicks"

  } else if (navigator.userAgent.match(/webOS/i)) {
    //code for webOS here
    console.log("webOS");
    window.location.href = "https://2clicks.uz/";

  } else {
    console.log("nomalum webOS");
    window.location.href = "https://2clicks.uz/";
  }
}

onMounted(() => {
  DetectIphone();
})

// DetectIphone();
</script>

<template>
  <div class="w-full p-15">
    <p>Hello world!</p>
  </div>
</template>
