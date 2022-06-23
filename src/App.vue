<template>
  <div id="app">
    <transition name="el-fade-in">
      <router-view/>
    </transition>
  </div>
</template>

<script>
export default {
  name: 'App',
  beforeCreate() {
    this.$store.dispatch('getAcount')
    console.log('即将拥有8块腹肌的HK')
  }
}
</script>

