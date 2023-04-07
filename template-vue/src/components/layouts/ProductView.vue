<script setup lang="ts">
import { onBeforeMount, ref } from "vue";
const result = ref();

const getProduct = () => {
  fetch("https://dummyjson.com/products?limit=3")
    .then((response) => response.json())
    .then((data) => {
      console.log("data", data);
      result.value = data.products;
    });
};

onBeforeMount(() => {
  getProduct();
});
</script>
<template>
  <div class="bg-green-lemon">
    <p class="text-center pt-5" style="font-size: 60px; font-weight: 700">
      LOREM IPSUM
    </p>
    <div class="py-5 d-flex justify-content-center">
      <div v-for="(item, k) in result" :key="k">
        <div class="card p-0 m-3 shadow rounded-0" style="width: 18rem; height: 400px">
          <img
            :src="`${item.thumbnail}`"
            style="height: 236px"
            alt="Card image cap"
          />
          <div class="card-body">
            <h5 class="card-title">{{ item.title }}</h5>
            <p class="card-text">
              {{ item.description }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
