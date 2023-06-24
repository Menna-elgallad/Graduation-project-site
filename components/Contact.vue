<template lang="pug">
.container-fluid
    .container
        .first 
            .left 
                h1
                    span &bdquo;
                    br 
                    
                    span Contact us
                p We value ypur feedback and inquiuries. please contact us using the following form 
            .right 
                .form
                    h3 Contact us
                    section
                        label(for="email") Email
                        input#email(type="email")
                    section
                        label(for="message") Message
                        textarea#message
                    .btn 
                            h6 send
        .second 
            h1(style="color: #FBC75E;") Smart Gate
            p(style="color: #A6A6A6; fontWeight: 300;") ANPR System for Univeristy
            h5 2023
            p(style="fontWeight: 400;") 
                span Faculty of Artificial Intlligence & Computer Science 
                span(style="float:right;") Damietta university

</template>

<script setup lang="ts"></script>

<style lang="scss" scoped>
.container-fluid {
  h1 {
    font-size: calc(4rem + 1vw - 30px);
  }
  background-color: #161c28;
  color: white;
  padding: 25px;
  .container {
    .left {
      p {
        color: #a6a6a6;
        margin-top: 5px;
      }
    }
    .first {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 20px;
      margin: 20px auto;
      .right {
        .form {
          float: right;
          background: #222938;
          display: flex;
          width: 100%;
          padding: 4rem;
          flex-direction: column;
          align-items: center;
          justify-content: center;
          border-radius: 10px;
          section {
            width: 100%;
            display: flex;
            flex-direction: column;
            input {
              border-radius: 10px;
              // height: 30px;
              width: 100%;

              padding: 0.7rem;
              border: none;
              margin-top: 1rem;
            }
            label {
              margin-top: 1rem;
            }
            textarea {
              border-radius: 10px;
              border: none;
              padding: 1rem;
              margin-top: 1rem;
              width: 100%;
            }
          }
          .btn {
            background: #fbc75e;
            color: white;
            border: none;
            height: 50px;
            width: 100%;
            display: grid;
            place-content: center;
            padding: 5px;
            align-items: center;
            border-radius: 10px;
            margin-top: 20px;
          }
        }
      }
    }
  }
  .second {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }
}
@media (max-width: 998px) {
  .container-fluid {
    .container {
      .second {
        text-align: center;
      }
      .first {
        display: grid;
        grid-template-columns: 1fr;
        .right {
          display: flex;
          justify-content: center;
        }
      }
    }
  }
}
</style>
