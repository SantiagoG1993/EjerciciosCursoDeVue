<template>
    <div>
        <h1 :style="'color:'+contadorColor" >Contador: {{contador}}</h1>
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
    color: brown;
}
</style>