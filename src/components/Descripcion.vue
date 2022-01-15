<template>
    <div class="descripcion">
        <div class="additem">
            <h2>Cantidad a pedir&nbsp;</h2>
            <div class="wrapper">
                <button class="btn" @click="cambiarContador('-1')" type="button" name="button">-</button>
                <input class="cantidad" type="text" name="name" :value="contador">
                <button class="btn" @click="cambiarContador('1')" type="button" name="button">+</button>
            </div>
            <button class="boton boton-alterno"><span class="material-icons">add_shopping_cart</span>&nbsp;Agregar al carro</button>
        </div>
        <h2>Descripción:</h2>
        <p>Trekking Bike equipado con un potente con motor central de la marca japonesa VINKA que te hará subir de nivel.</p>

        <p>Una bicicleta eléctrica versátil, pensada para tus trayectos en la ciudad y también para disfrutar de fantásticos paseos en tu tiempo libre.</p>

        <p>Disfruta al aire libre con este modelo Biwbik de la línea de bicicletas eléctricas de Trekking. La comodidad del pedaleo asistido te permitirá hacer deporte y disfrutar de tus momentos de ocio, sin necesidad de realizar sobreesfuerzos.</p>

        <p>Batería y cargador incluidos.</p>

        <p>Como todos los modelos Biwbik, dispone de la Certificación 15194, la normativa Europea que certifica la seguridad de las bicicletas con asistencia eléctrica.</p>

        <iframe width="560" height="315" src="https://www.youtube.com/embed/LTdY9yRymp8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
 

        <h2>Características:</h2>
        <ul>
            <li>GENERAL: Bicicleta eléctrica Trekking/Paseo. Cuadro de aluminio 27,8 x 18″</li>
            <li>MOTOR/CAMBIOS: VINKA E40N, 250W – 80Nm 110Rpm Sensor Torque Vinka DR23 / Shimano Altus ARDM310DLC</li>
            <li>MANETA: Shimano Altus ASLM310R8A Rapidfire – 8 speed</li>
            <li>FRENOS: Frenos de disco hidráulicos Shimano MT200 (delantero y trasero)</li>
            <li>RUEDAS: 27,5″ x 2,10″</li>
            <li>AUTONOMÍA/BATERÍA: SAMSUNG 36V 14Ah (504Wh)</li>
            <li>ACCESORIOS: Guardabarros. Faro delantero. Display LCD</li>
            <li>GARANTÍA: Garantía bicicleta: 2 años – Garantía batería/cargador: 1 año</li>
        </ul>
        
    </div>
</template>

<script>
export default {
    name: "Descripcion",
    data () {
        return {
            contador: 1
        }
    },
    methods: {
        cambiarContador(num) {
            this.contador += +num;
            if (!isNaN(this.contador) && (this.contador < 0)) {
              this.contador = 0
            }
        }
    }
}
</script>

<style>
    .additem {
        display: flex;
        align-items: center;
    }
    .wrapper {
    height: 2rem;
    display: flex;
    }

    .cantidad {
    border: none;
    text-align: center;
    width: 2rem;
    font-size: 1.2rem;
    border: 1px solid #d8d8d8;
    }
    .btn {
    border: 1px solid #d8d8d8;
    width: 1.8rem;
    }
    .descripcion button:hover {
        background-color: rgb(250, 180, 0);
        color: rgb(41,120,128);
    }
</style>