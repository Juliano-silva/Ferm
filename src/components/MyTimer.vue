<template>
  <div id="Corpo5">
    <br>
    <h1>Tempo para acabar o mês</h1>
<div id="Relogio">
  <Countdown countdownSize="15vh" labelSize="5vh" labelColor="white"/>
</div>
</div>
</template>

<script>
import {Countdown} from 'vue3-flip-countdown'
export default {
  name: 'App',
  components: {
    Countdown
  }
}
</script>
