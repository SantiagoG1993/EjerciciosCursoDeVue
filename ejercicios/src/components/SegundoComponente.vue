<template>
    <div class="container__contador">
        <h1>Contador: <span :style="'color:'+contadorColor">{{contador}}</span></h1>
        <button @click="contador--">-</button>
        <button @click="contador++">+</button>
    </div>
</template>

<script>
export default {
    data(){
        return{
            contador:0
        }
    },
    computed:{
        contadorColor(){
            if(this.contador < 0){
                return 'red'
            }
            if(this.contador > 0){
                return 'green'
            }
            else{
                return 'black'
            }
        }
    }
}
</script>

<style scoped>
h1{
    color: black;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 40px;
}
.container__contador{
    width: 450px;
    border-radius: 8px;
    display: flex;
    background-color: rgb(242, 242, 242);
    margin-top: 20px;
   box-shadow: 1px 1px 20px 1px rgb(190, 190, 190) ;
}
button{
    width: 90px;
    margin-left: 10px;
    border: none;
    font-size: 30px;
    border-radius: 8px;
    background-color: aquamarine;
}
button:hover{
    cursor: pointer;
    background-color: orange;
}
</style>