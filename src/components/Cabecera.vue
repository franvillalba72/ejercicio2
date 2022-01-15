<template>
    <header id="cabecera">
        <img alt="Logotipo de biciSHOP" src="../assets/bicishop-logo.png">
        <nav id="menu-principal">
            <a href="#">Inicio</a>
            <a href="#">Tienda</a>
            <a href="#">Equipo</a>
            <a href="#">Salidas</a>
        </nav>
        <div id="botones">
            <button class="boton"><span class="material-icons">login</span>&nbsp;Login</button>
            <button class="boton"><span class="material-icons">manage_accounts</span>&nbsp;Registro</button>
        </div>
    </header>
</template>

<script>
export default {
    name: "Cabecera"
}
</script>

<style>
    #cabecera {
        padding: 1em;
        background-color: rgb(41, 120, 128);
        display: flex;
        align-items: center;
    }

    #cabecera img {
        width: 300px;
    }

    #menu-principal {
        text-align: center;
        flex-grow: grow;
        justify-content: space-between;
        margin: 0 auto;
    }

    #menu-principal a {
        color: rgb(250,180,0);
        margin: 0 1em 0 1em;
        font-size: 1.5em;
    }

    #botones {
        display: flex;
    }

    #botones button:hover {
        color: rgb(250, 180, 0);
        background-color: rgb(41,120,128);
    }
</style>