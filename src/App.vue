<template>
  <div id="app">
    <h2>Registro de personas</h2>
    <TablaClaseCuatro :titulos="tabla1.titulos" :registros="tabla1.registros" >
    </TablaClaseCuatro>
    <h2>Productos</h2>
    <TablaClaseCuatro :titulos="tabla2.titulos" :registros="tabla2.registros">
    </TablaClaseCuatro>
    <h2>Ranking ATP</h2>
    <TablaClaseCuatro :titulos="tabla3.titulos" :registros="tabla3.registros">
    </TablaClaseCuatro>
  </div>
</template>

<script>
import TablaClaseCuatro from './components/TablaClaseCuatro.vue'; 

export default {
  name: 'App',
  components: {
    TablaClaseCuatro
  },
  data(){
        return{
            tabla1: {
            titulos: ["DNI","Nombre", "Apellido", "Estado civil"],
            registros: [
                ["35.459.554","Jeremias", "Orcajo", "Casado"],
                ["29.659.996","Juliana", "Etchanchu", "Soltero"],
                ["21.344.567","Marisol", "Sanchez", "Casado"],
                ["21.545.284","Eugenia", "Melazco", "Casado"],
            ]
        },
        tabla2: {
            titulos: ["Producto", "Disponible", "Valor"],
            registros: [
                ["Leche", "Si", "$150"],
                ["Yerba", "No", "$250"],
                ["Arroz", "Si", "$170"],
                ["Pan", "Si", "$40"],
            ]
        },
        tabla3: {
            titulos: ["Posicion", "Tenista", "Puntos"],
            registros: [
                ["1°", "Novak Djokovic", "8400"],
                ["2°", "Daniil Medvedev", "8080"],
                ["3°", "Alexander Zverev", "7420"],
                ["4°", "Rafael Nadal", "6435"],
            ]
        },
        }
  }
  
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
