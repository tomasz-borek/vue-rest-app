<template>
    <nav>
        <div id="logo">
            <img src="../assets/navbarLogo.png">
        </div>
        <div>New Vue Apllication!</div>
    </nav>
</template>

<script>
export default {
    name:"NavigationBar",
}

</script>

<style lang="scss">
nav {
    background-color: #EEEEEE;
    div {
        margin-right: 20px;

        img {
            max-width: 200px;
        }
        font-size: 24px;
    }
}
</style>