<template>
  <header class="header">
    <ul>
        <li><nuxt-link :to="{ path: '/' }">Home</nuxt-link></li>
        <li><nuxt-link :to="{ name: 'users' }">Users</nuxt-link></li>
    </ul>
  </header>
</template>

<style scoped>
    .header{
        width:100%;
        height:60px;
        display:flex;
        justify-content:center;
        align-items: center;
    }
    .header ul li{
        display:inline-flex; 
        margin-right: 5px;  
    }

</style>