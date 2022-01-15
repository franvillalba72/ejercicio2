<template>
    <div id="breadcrumb">
        <a href="#"><span class="material-icons">home</span> </a>
        <a href="#"> Tienda </a>
        <a href="#" class="actual"> Bicicletas, e-bikes</a>
    </div>
</template>

<script>
export default {
    name: "Breadcrumb"
}
</script>

<style>
    #breadcrumb {
        display: flex;
        align-items: center;
        margin: 1em;
    }

    #breadcrumb a {
        color: rgb(41, 120, 128);
        padding: 0 1em;
        border-right: solid 1px;
        font-size: 1.5em;
    }

    #breadcrumb a.actual {
        font-weight: bold;
    }
</style>