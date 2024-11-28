<template>
  <div id="app">
    <BasicLayout />
  </div>
</template>

<style></style>
<script setup lang="ts">
import BasicLayout from "@/layouts/BasicLayout.vue";
import { useLoginUserStore } from "@/store/userLoginUserStore";

const loginUserStore = useLoginUserStore();
loginUserStore.fetchLoginUser();
</script>
