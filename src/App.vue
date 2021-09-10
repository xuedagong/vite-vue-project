<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import HelloWorld from './components/HelloWorld.vue'
import MyInfo from './components/MyInfo.vue'
import naive from "naive-ui";
</script>

<template>
  <n-space vertical size="large">
    <n-layout has-sider>
      <n-layout-sider
        collapse-mode="transform"
        :width="240"
        show-trigger="bar"
        content-style="padding: 24px;"
        bordered
      >
       <router-link to="/">Go to Home</router-link> 
       <br>
       <router-link to="/about">Go to About</router-link>
       <br>
       <router-link to="/table">Go to TableList</router-link>
      </n-layout-sider>
      <n-layout-content style="padding:10px;border:1px solid;"><router-view></router-view></n-layout-content>
    </n-layout>
  </n-space>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
