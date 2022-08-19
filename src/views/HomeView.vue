<template>
  <!-- <div class="home"> -->
  <div class="container">
    <h2 class="header">SQL Cookbook</h2>
    <h6 class="sub_header">Your journy to SQL mastery</h6>
    <img class="img" src = "../assets/homepage_svg.svg" alt="My Happy SVG"/>

    <div class="actions_container">
        <div class="action" v-for="action in actions" :key="action.name">        
                         <h2>{{action.name}}</h2>
        </div>
        
    </div>
    <p>see all</p>
</div>
  <!-- </div> -->
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    // HelloWorld
  }
}
</script>

