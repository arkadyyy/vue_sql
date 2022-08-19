<template>
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
    
</template>

<script>
    export default {
        name : 'HomePage',
        data() {
            return{
                actions : [
                    {name: 'hello'},
                    {name : 'world'},
                    {name : 'world'},
                    {name : 'world'},
                    {name : 'world'},
                    ]
            }
               
        }
       

    }
</script>

<style>
    .container {
        height: 100vh;
        background-color: '#f4f4f4';
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    .header {
        color: rgba(52, 47, 47, 0.5);
        font-weight: lighter;
    }
    .sub_header {
       margin-block-start: 0;
       margin-block-end: 0;
         
    }
    .img {
        width: 400px;
        height: 330px;
        
    }
    .actions_container {
        display: flex;
        flex-direction: row;
    }
    .action { 
        border-width: 1px;
        border-style: solid;
        border-color: gray;
        border-radius: 12px;
        margin: 20px;
        padding: 20px;
    }
</style>