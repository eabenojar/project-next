<template>
    <div class="sidebar-container">
        <div class="sidebar-img-container">
            <h1>EA</h1>
            <img src="" alt="">
        </div>
        <div class="sidebar-list">
  <ul ><li class="sidebar-list__title" v-for="(item,index) in items" v-bind:key="index">{{item.name}}</li></ul>
        </div>
      
    </div>
</template>

<script>
export default {
    data: function(){
        return {
items: [
             {name: "About"},
            {name: "Projects"},
            {name: "Work"},
            {name: "Contact"},
        ]
        }
        
    }
}
</script>

<style scoped>
ul {
    list-style-type: none;
    padding: 0;
}
    .sidebar-container {
        background-color: #F1F1F1;
        width: 20%;
        height: 100vh;
    }
    .sidebar-list__title {
        height: 80px;
        border-bottom: 1px solid #E3E3E3;
        font-family: sans-serif;
        font-weight: 600;
        display: flex;
        align-items: center;
        padding: 1rem;
         color: #8E8E8E;
    }
     .sidebar-list__title:hover {
        color: #0E0E0E;
    }
    .sidebar-img-container {
        height: 80px;
        background-color: #65BF9D;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>
