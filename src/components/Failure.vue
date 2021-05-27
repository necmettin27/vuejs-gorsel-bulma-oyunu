<template>
  <div class="container">
      <h1>Malesef Bilemediniz!!!</h1>
      <button @click="newGame">Yeni Oyun</button>
  </div>
</template>
<script>
export default {
    methods:{
        newGame(){
            this.$emit('isCorrectevent','app-game-cards');
        }
    }
}
</script>
<style scoped>
    .container{
        position: absolute;
        top: 0px;
        left: 0px;
        width: 100%;
        height: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-color: darkred;
    }
    .container h1{
        text-align: center;
        font-size: 333%;
        color:white;
    }
    .container button{
        width: 200px;
        background-color: #fff;
        color:darkred;
        border:1px solid brown;
        font-size: 15px;
        outline: none;
        border-radius: 5px;
        height: 50px;
         transition: all .5s;
         cursor: pointer;
    }
    .container button:hover{
        background-color: lightgreen;
        color:#fff;
        transition: all .5s;
    }
</style>