<script setup>

</script>

<template>
    <div class="wrap">
            <nav>
                    <ul>
                        <li><a href="#home">Home</a></li>
                        <li><a href="#news">News</a></li>
                        <li><a href="#contact">Contact</a></li>
                        <li><a href="#about">About</a></li>
                    </ul>
            </nav>
            <div>
                html ana sayfa
                <router-view></router-view>
    
            </div>
    
        </div>
</template>

<style scoped>
.wrap{
    display: flex;
}

nav{
    display: flex;
    width: 23%;
    background-color: red;
}
template{
    display: flex;
}
</style>