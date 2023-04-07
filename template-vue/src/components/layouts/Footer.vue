<script setup lang="ts">
import { DatePicker } from 'ant-design-vue';
</script>
<template>
  <div class="p-6 bg-dark">
    <div class="row">
      <div class="col-6">
        <div class="d-flex align-items-center justify-content-center">
          <img
            src="../../assets/Bicycleimg.svg"
            style="width: 719px; height: 423px"
            alt="Bicycle"
          />
        </div>
      </div>
      <div class="col-6">
        <p
          class="pt-5 text-white"
          style="font-size: 60px; font-weight: 700"
        >
          ติดต่อเรา
        </p>
        <form class="form-inline">
          <div class="form-group mb-2">
            <input
              type="text"
              class="form-control-plaintext"
              placeholder="ชื่อ - นามสกุล"
            />
          </div>
          <div class="form-group mb-2">
            <input
              type="text"
              class="form-control-plaintext"
              placeholder="เบอร์ติดต่อ"
            />
          </div>
          <div class="form-group mb-2">
            <input
              type="text"
              class="form-control-plaintext"
              placeholder="อีเมล"
            />
          </div>
          <div class="form-group mb-2">
            <input
              type="date"
              placeholder="อีเมล"
              class="form-control-plaintext"
            />
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<style>
input.form-control-plaintext {
    display: block;
    width: 50%;
    padding: 0.375rem 0;
    margin-bottom: 0;
    line-height: 1.5;
    color: #ffffff;
    background-color: transparent;
    /* border: solid transparent; */
    border-width: 1px 0;
    border-bottom: 1px solid #ffffff;
}
</style>
