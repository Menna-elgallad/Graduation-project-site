<template lang="pug">
.container-fluid 
   
    .container

        h1 
            span Meet the 
            span(style="color: #FBC75E;") team 
        p And thier rules
        .members
            .member(v-for="i in data")
                .image
                    img(:src="i.avatar")
                .names 
                    h4 {{ i.fName }}
                    p {{ i.lName }}
                    

        
        
</template>

<script setup lang="ts">
import data from "../team.json";
</script>

<style lang="scss" scoped>
h1 {
  font-size: calc(4rem + 1vw - 30px);
}
.container-fluid {
  margin-top: 40px;
  background-color: #fafafa;
  padding-top: 20px;

  .container {
    margin-top: 30px;

    display: flex;
    flex-direction: column;
    align-items: center;
    .members {
      margin-bottom: 30px;
      display: grid;
      grid-template-columns: repeat(5, 1fr);
      gap: 50px;
      .member {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: center;
        .image {
          margin-top: 30px;
        }
        .names {
          display: flex;
          flex-direction: column;
          justify-content: space-between;
          align-items: center;
          margin-top: 1rem;
        }
      }
    }
  }
}
@media (max-width: 998px) {
  .container-fluid {
    .container {
      .members {
        display: grid;
        gap: 10px;
        grid-template-columns: 1fr 1fr;
        place-content: center;
        .member {
          width: 150px;

          .image {
            width: 130px;
          }
          .names {
            display: flex;
            align-items: center;
            justify-content: center;
          }
        }
      }
    }
  }
}
</style>
