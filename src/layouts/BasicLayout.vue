<script setup lang="ts">
import GloblHeader from "@/components/GloblHeader.vue";
import { getCurrentUser } from "@/api/user";

// getCurrentUser().then((res) => {
//   console.log(res);
// });
</script>

<template>
  <div id="basic-layout">
    <a-layout>
      <a-layout-header class="Header">
        <GloblHeader />
      </a-layout-header>
      <a-layout-content class="content">
        <router-view />
      </a-layout-content>
      <a-layout-footer class="footer">
        <a href="https://codefather.cn" target="_blank"> 编程导航 </a>
      </a-layout-footer>
    </a-layout>
  </div>
</template>

<style scoped>
#basic-layout .footer {
  background: #efefef;
  text-align: center;
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  padding: 16px;
}

#basic-layout .content {
  padding: 20px;
  margin-bottom: 20px;
  background: linear-gradient(to right, #fefefe, #fff);
}

#basic-layout .Header {
  background: white;
  margin-bottom: 10px;
  color: unset;
  padding-inline: 20px;
}
</style>
