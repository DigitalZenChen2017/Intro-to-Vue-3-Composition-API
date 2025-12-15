<script setup>
import { ref } from "vue";

const productTitle = ref("Socks");
const productDescription = ref("A pair of warm, fuzzy socks.");
</script>

<template>
  <div class="product-display">
    <div class="product-container">
      <div class="product-info">
        <h1>{{ productTitle }}</h1>
        <p>{{ productDescription }}</p>
      </div>
    </div>
  </div>
</template>
