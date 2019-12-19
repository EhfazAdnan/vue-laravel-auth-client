<template>
    <ul>
        <li><router-link :to="{name:'home'}">Home</router-link></li>
        <li><router-link :to="{name:'signin'}">Sign In</router-link></li>
        
        <li>Ehfaz Ahmed Adnan</li>
        <li><router-link :to="{name:'dashboard'}">Dashboard</router-link></li>
        <li><a href="#">Sign Out</a></li>
    </ul>
</template>