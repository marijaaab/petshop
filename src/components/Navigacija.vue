<template>
     <div id="nav">
         <nav class='navbar'>
             <a class="navbar-brand" href='#'>
                 <img src="../assets/logo.png">
             </a>
             <div class="navbar-menu">
                <router-link to="/">Home</router-link> |
                <router-link to="/about">About</router-link>
             </div>
         </nav>
     
    </div>
</template>

<style>
    #nav{
        background-color: lightgrey;
    }

    #nav img{
        width: 40px;
        height: 40px;
    }

    .router-link-exact-active{
        color: #e959e4 !important;
    }

</style>

<script>
    export default{
        name: 'Navigavija'
    }
</script>