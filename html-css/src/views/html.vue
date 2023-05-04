<script setup>

</script>

<template>
    <div class="container">
        <router-link to="/boxsizing" tag="a" class="link">Anasayfa</router-link>
        <div>
            <b-button-group>
                <b-button>Button</b-button>
                <b-dropdown right text="Menu">
                    <router-link to="/boxsizing" tag="b-dropdown-item" class="link">Box-Sizing</router-link>
                    <b-dropdown-item>Item 1</b-dropdown-item>
                    <b-dropdown-item>Item 2</b-dropdown-item>
                    <b-dropdown-divider></b-dropdown-divider>
                    <b-dropdown-item>Item 3</b-dropdown-item>
                </b-dropdown>
                <b-dropdown right split text="Split Menu">
                    <b-dropdown-item>Item 1</b-dropdown-item>
                    <b-dropdown-item>Item 2</b-dropdown-item>
                    <b-dropdown-divider></b-dropdown-divider>
                    <b-dropdown-item>Item 3</b-dropdown-item>
                </b-dropdown>
            </b-button-group>
        </div>
        <div class="wrap">
            <div>
                html ana sayfa
                <router-view></router-view>
            </div>

        </div>
    </div>
</template>

<style scoped>
.wrap {
    display: flex;
}

nav {
    display: flex;
    width: 23%;
    background-color: red;
}

template {
    display: flex;
}
</style>