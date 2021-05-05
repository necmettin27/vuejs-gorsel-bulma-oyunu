<template>
<component
  :is="activeComponent"
></component>
</template>

<script>
import GameCards from './components/GameCards'
import Failure from './components/Failure'
import Celebrate from './components/Celebrate'
export default {
  data(){
    return{
      activeComponent: 'appGameCards'
    }
  },
  components:{
    appGameCards : GameCards,
    appCelebrate : Celebrate,
    appFailure : Failure
  }
}
</script>

<style>
body{
   font-family: sans-serif;
}
</style>
