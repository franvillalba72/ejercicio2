<template>
    <footer id="piepagina">
        <div class="derechos">
            <h3>biciSHOP &copy; 2022 - Todos los derechos reservados</h3>
        </div>
        <div class="redes">
            <img src="../assets/facebook24.png" alt="Icono de facebook">
            <img src="../assets/instagram23.png" alt="Icono de instagram">
            <img src="../assets/twitter24.png" alt="Icono de twitter">
        </div>
    </footer>
</template>

<script>
export default {
    name: "Piepagina"
}
</script>

<style>
    #piepagina {
        padding: 1em;
        background-color: rgb(41, 120, 128);
        color: rgb(250,180,0);
        display: flex;
        align-items: center;
    }

    .derechos {
        padding: 1em;
        flex-grow: grow;
        margin: 0 auto;
    }

    .redes {
        padding: 1em;
        display: flex;
        justify-content: space-between;
    }

    .redes img {
        margin: 0 1em;
    }
</style>