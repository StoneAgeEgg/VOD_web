<template>
  <!-- <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/>
  </div> -->

 <el-container>
   <el-header>
      <Header/>
    </el-header>
    <el-container>
      <el-main>
        <Show/>
      </el-main>

     <el-aside width="200px">
        <Aside/>
      </el-aside>
    </el-container>
  </el-container>

</template>

<script lang="ts">
import {Options, Vue} from 'vue-class-component';
// import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src
import Show from '@/components/Show.vue';
import Header from '@/components/Header.vue';
import Aside from '@/components/Aside.vue';

@Options({
  components: {
    // HelloWorld,
    Header,
    Show,
    Aside,
  },
})
export default class Home extends Vue {
}
</script>

<style lang="scss">
.el-header {
  height: auto;
  background: black;

}

</style>

