<template lang="pug">
.container
    h1 
        span Watch the 
        span(style="color: #FBC75E;") live 
        span demo 
    iframe.frame(src="/assets/sg-website/")

</template>

<script setup lang="ts">
</script>

<style scoped lang="scss">
.container {
  h1 {
    font-size: calc(4rem + 1vw - 30px);
  }
  margin-top: 50px;
  display: flex;
  flex-direction: column;
  align-items: center;
  .frame {
    width: 80%;
    margin-top: 50px;
    height: 400px;
  }
}
@media (max-width: 998px) {
  .container {
    .frame {
      width: 80%;
    }
  }
}
</style>