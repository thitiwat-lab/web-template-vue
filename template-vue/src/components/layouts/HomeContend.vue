<script setup lang="ts">
import ContendProfile from './ContendProfile.vue'
import ProductView from './ProductView.vue'
</script>

<template>
  <div class="bg-dark">
      <div class="row pb-6">
        <div class="col-5 d-flex justify-content-end">
          <div class="d-flex justify-content-center text-white">
              <col-3>
              <p style="font-size:96px; font-weight: 700; padding: 0; margin-bottom: 0;">LOREM</p>
              <p class="text-green-lemon" style="font-size:96px; font-weight: 700; padding: 0; margin-bottom: 0; color: ;">IPSUM</p>
                <p style="font-size:18px; margin-bottom: 0; font-weight: 600;">Lorem Ipsum is simply Lorem Ipsum is</p>
                <p style="font-size:18px; margin-bottom: 0; font-weight: 600;">simply Lorem Ipsum is simply</p>
                <p style="font-size:18px; margin-bottom: 0; margin-top: 15px;">Lorem Ipsum is simply dummy text of</p>
                <p style="font-size:18px; margin-bottom: 0;">the printing and typesetting industry. Lorem Ipsum</p>
                <p style="font-size:18px; margin-bottom: 0;">has been the industry's</p>
              </col-3>
          </div>
        </div>
        <div class="col-7">
            <img src="../../assets/Bicycleimg.svg" alt="Bicycle">
        </div>
      </div>
      <ContendProfile/>
  </div>
  <ProductView/>
</template>
