<template>
  <div class="gameboy">
    <div class="frame">
      <div class="screen">
        <Nuxt />
      </div>
    </div>
    <Controller></Controller>
  </div>
</template>

<script>
import Controller from  '~/components/Controller'
export default {
  components: {
    Controller,
  },
}
</script>

<style>
.frame{
  background: gray;
  padding: 16px 20px 20px;
  border-radius: 4px;
}
.screen{
  height: 50vh;
  background: #FFFAF0;
  padding: 16px;
  border-radius: 4px;
}
</style>