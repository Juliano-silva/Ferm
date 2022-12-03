<template>
  <MyHeader/>
  <MyApiVue/>
  <MyApiExterna/>
  <MyGaleria/>
  <MyPageWeb/>
  <MyTimer/>
</template>

<script>
import { defineComponent } from 'vue'
import MyApiVue from './components/MyApi.vue';
import MyApiExterna from './components/MyApiExterna.vue';
import MyGaleria from './components/MyRoleta.vue';
import MyPageWeb from './components/MyPageWeb.vue';
import MyTimer from './components/MyTimer.vue';
import MyHeader from './components/MyHeader.vue';
export default defineComponent({
  name: 'App',
  components:{
    MyApiVue,
    MyApiExterna,
    MyGaleria,
    MyPageWeb,
    MyTimer,
    MyHeader
  }
})
</script>
