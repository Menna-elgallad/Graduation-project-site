<template lang="pug">
.container 
    .left 
        h1 
            span Automatic
            br
            span Number Plate
            br
            
            span  Recognition 
        img(src="/vector 1.png")
        p(style="margin-top:1rem  ; color: black ; font-weight  : bold")
            span Automatic ANPR system is for university which 
            br
            span enables effecient and automated identification of
            br
            span registerd vehicles
        .btns
            .btn 
                nuxt-link.link(to="#about") learn more
            .btn2
                nuxt-link.link(to="#demo") 
                    IconsPlay/ {{ " " }} view demo
    .right 
        img(src="/p1.png")

</template>

<script setup lang="ts">
</script>

<style scoped lang="scss">
.container {
  display: flex;
  background-color: #fafafa;
  justify-content: space-between;
  align-items: center;
  margin: 40px auto;
  .left {
    padding: 3rem;
    font-size: larger;
    transform: scaleY(1.1);
    line-height: 25px;
    p {
      @media (max-width: 998px) {
        text-align: center;
        font-size: small;
      }
    }
    h1 {
      font-weight: 600;
      font-size: calc(4rem + 1vw - 20px);
      @media (max-width: 998px) {
        text-align: center;
      }
    }
    img {
      margin-top: 20px;
      margin-bottom: 10px;
    }
    .btns {
      display: flex;
      align-items: center;
      gap: 25px;
      margin-top: 10px;
      @media (max-width: 998px) {
        justify-content: center;
      }
      @media (max-width: 420px) {
        flex-direction: column;
      }
      .btn {
        background: #fbc75e;
        color: white;
        border: none;

        place-content: center;
        padding: 0.5rem 1rem;

        border-radius: 20px;
        margin-top: 20px;
      }
      .btn2 {
        border: none;
        height: 30px;

        display: grid;
        place-content: center;
        padding: 5px;
        align-items: center;
        border-radius: 20px;
        margin-top: 20px;
      }
    }
  }
}
@media (max-width: 998px) {
  .container {
    margin-top: 70px;
    display: flex;
    flex-direction: column;
    grid-template-columns: 1fr;
    .right {
      width: 77%;
      margin-top: 50px;
    }
  }
}
a {
  margin: 0;
  padding: 0;
}
</style>
