<script setup>
import { ref } from "vue";
import sockGreenImage from "./assets/images/socks_green.jpeg";
import sockBlueImage from "./assets/images/socks_blue.jpeg";

const product = ref("Socks");
const greenSockImage = ref(sockGreenImage);
const blueSockImage = ref(sockBlueImage);
const greenSockLink = ref("https://example.com/green-socks");
const blueSockLink = ref("https://example.com/blue-socks");
</script>

<template>
  <div class="product-display">
    <div class="product-container">
      <div class="product-image">
        <!-- image goes here -->
        <img :src="greenSockImage" alt="Green Socks" />
        <a :href="greenSockLink" target="_blank"
          >Purchase Green Christmasy Socks Here!</a
        >
        <img :src="blueSockImage" alt="Blue Socks" />
        <a :href="blueSockLink" target="_blank">Buy Navy Manly Socks Here!</a>
      </div>
      <div class="product-info">
        <h1>{{ product }}</h1>
      </div>
    </div>
  </div>
</template>
