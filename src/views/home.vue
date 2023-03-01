<template>
  <div class="home">
    <p>{{ myTheme.themeColor }}</p>
  </div>
</template>
<script setup lang="ts">
import theme from '@/store/theme'
const myTheme = theme()
myTheme.setThemeType('暗淡色')
</script>

<style lang="less" scoped>
.home {
  background: darkblue;
  p {
    color: #ddd;
  }
}
</style>
