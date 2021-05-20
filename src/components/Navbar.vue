<script setup>
import BSSLogo from '../assets/BSSLogo.vue';
import StoolAndStars from '../assets/StoolAndStars.vue';
</script>

<template>
  <div class="navbar-container">
    <div class="left">
      <BSSLogo />
      <span class="divider"></span>
      <span class="navbar-title">Reviews</span>
    </div>
    <div class="right">
      <StoolAndStars />
    </div>
  </div>
</template>

<style>
.navbar-container {
  background-image: linear-gradient(275deg, #102442 105%, #06101e -11%);
  height: 90px;
  display: flex;
  overflow-y: hidden;

  --tw-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
  box-shadow: var(0, 0 0 #0000), var(0, 0 0 #0000), var(--tw-shadow);
}

.left {
  display: flex;
  flex: 1;
  align-items: center;
  height: 100%;
  padding-left: 16px;
}

.left > svg {
  height: 58px;
  width: 135px;
}

.divider {
  margin-left: 16px;
  margin-right: 16px;
  width: 0px;
  height: 58px;
  opacity: 0.4;
  border: solid 1px #ffffff;
}

.navbar-title {
  font-size: 22px;
  color: #ffffff;
}

.right > svg {
  width: 240px;
  height: 240px;
  margin-top: -50px;
  margin-right: -24px;
}
</style>