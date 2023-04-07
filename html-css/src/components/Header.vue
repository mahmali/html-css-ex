<script setup>

</script>

<template>
    <nav>
        <div class="container">
            <ul>
                <li>
                    <router-link to="/" tag="a" class="link">Anasayfa</router-link>
                </li>
                <li>
                    <router-link to="/form" tag="a" class="link">Form</router-link>
                </li>
                <li>
                    <router-link to="/html" tag="a" class="link">Html-Css</router-link>
                </li>
                <li><a href="contact.asp">Contact</a></li>
                <li><a href="about.asp">About</a></li>
            </ul>
        </div>

    </nav>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100&display=swap');

nav {
    width: 100%;
    background-color: #333;
}

ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
    background-color: #333;
}

li {
    float: left;
}

li a {
    display: block;
    color: white;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
}

/* Change the link color to #111 (black) on hover */
li a:hover {
    background-color: #111;
}
</style>