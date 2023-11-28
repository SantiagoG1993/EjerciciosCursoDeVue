<template>
    <div class="componente1">
        <h1>Mi nombre es: {{nombre}}</h1>
        <input @keyup.enter="agregarNombre"  id="input_text" v-model="nombreCapturado" type="text" placeholder="ingrese su nomnbre">
        <button @click="agregarNombre" id="btn_cambiar" >Cambiar nombre</button>
        <button @click="borrarNombre" id="btn_cambiar" >Borrar nombre</button>
    </div>
</template>


<script>
export default {
    data(){
        return{
            nombre:'',
            nombreCapturado:''
        }
    },
    methods:{
        agregarNombre(){
            this.nombre = this.nombreCapturado.toUpperCase()
        this.nombreCapturado = ""
        },
        borrarNombre(){
            this.nombre = ''
        }
    }
}
</script>


<style scoped>
.componente1{
    border-radius: 8px;
    background-color: rgb(238, 238, 238);
    width: 300px;
    height: 250px;
    display: flex;
    flex-direction:column;
    align-items: center;
    font-family: Arial, Helvetica, sans-serif;
    box-shadow: 1px 1px 20px 1px rgb(190, 190, 190) ;
}
h1{
    color: green;
    font-size: 20px;
}
#btn_cambiar{
    width: 150px;
    height: 40px;
    border: none;
    margin-top: 20px;
    background-color: rgb(72, 82, 82);
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    border-radius: 4px;
    cursor: pointer;
}
#btn_cambiar:hover{
   background-color: rgb(102, 110, 110); 
}
#input_text{
    width: 200px;
    height: 50px;
    text-align: center;
    border: none;
    cursor: pointer;
}
#input_text:focus{
    outline: none;
}
</style>