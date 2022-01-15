<template>
    <section id="imagenes">
        <div class="img-mini">
            <a @click="cambiarFoto(1)"><img v-bind:src="fotos[1]" alt="E-Bike Trekking Biwbik LANS"/></a>
            <a @click="cambiarFoto(2)"><img v-bind:src="fotos[2]" alt="E-Bike Trekking Biwbik LANS"/></a>
            <a @click="cambiarFoto(3)"><img v-bind:src="fotos[3]" alt="E-Bike Trekking Biwbik LANS"/></a>
            <a @click="cambiarFoto(4)"><img v-bind:src="fotos[4]" alt="E-Bike Trekking Biwbik LANS"/></a>
            <a @click="cambiarFoto(5)"><img v-bind:src="fotos[5]" alt="E-Bike Trekking Biwbik LANS"/></a>
        </div>
        <div class="img-big">
            <img v-bind:src="fotos[0]" alt="E-Bike Trekking Biwbik LANS" />
        </div>
    </section>
</template>

<script>
export default {
  name: "Imagenes",
  data() {
    return {
      fotos: [
        require("../assets/lans-600x600.jpg"),
        require("../assets/lans-600x600.jpg"),
        require("../assets/lans2-600x600.jpg"),
        require("../assets/lans3-600x600.jpg"),
        require("../assets/lans11-600x600.jpg"),
        require("../assets/lans16-600x600.jpg"),
      ],
    };
  },
  methods: {
    cambiarFoto(id) {
      this.fotos[0] = this.fotos[id];
    },
  },
};
</script>

<style>
#imagenes {
    display: flex;
    border-radius: 25px;
    padding: 1rem;
    margin: 1rem;
}
.img-big {
    flex-grow: grow;
    width: 600px;
    height: 600px;
    margin-right: 5em;
}
.img-mini {
    display: flex;
    flex-direction: column;
    /*justify-content: space-between;*/
    align-items: flex-start;
}
.img-mini img {
  width: 100px;
  border: 1px solid;
  margin-bottom: 1.5em;
}
</style>
