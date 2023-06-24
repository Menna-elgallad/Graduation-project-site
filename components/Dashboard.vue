<template lang="pug">
.container-fluid 
    .container
        .left 
            img(src="/lap.png")
        .right 
            h1 Dashboard System 
            p in addition, we have developed a dashboard system to improve security and controlling the gate, this feature empowers the adminstrator to have comprehensive control. 
            .btn 
            
                a.link(href="https://board-smartgate.onrender.com/") view
</template>

<script setup lang="ts">
</script>

<style lang="scss" scoped>
.container-fluid {
  background-color: #fafafa;
  .container {
    margin-bottom: 50px;
    display: grid;
    grid-template-columns: 1fr 1fr;
    align-items: center;
    .right {
      h1 {
        margin-bottom: 20px;

        font-size: calc(4rem + 1vw - 30px);
      }
      p {
        color: #a6a6a6;
      }
      .btn {
        background: #fbc75e;
        color: white;
        border: none;

        place-content: center;
        padding: 0.5rem 1.2rem;
        border-radius: 20px;
        margin-top: 20px;
      }
      a {
        margin: 0;
        padding: 0;
      }
    }
  }
}
@media (max-width: 998px) {
  .right {
    text-align: center;
  }

  .container-fluid {
    .container {
      display: grid;
      grid-template-columns: 1fr;
    }
  }
}
</style>