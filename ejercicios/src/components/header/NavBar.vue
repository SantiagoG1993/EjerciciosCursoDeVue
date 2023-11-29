<template>
    <div class="navbar">
        <div class="search_bar_logo">
            <img id="logo" src="ml-logo.svg" alt="">
            <div class="searchbar">
                <input type="text" placeholder="Buscar productos, marcas y mas...">
                <span id="barra">|</span>
                <i class="fa-solid fa-magnifying-glass"></i>
            </div>
                <img id="disney_promo" src="https://http2.mlstatic.com/D_NQ_957153-MLA69318147677_052023-OO.webp" alt="">

        </div>
        <div class="envio_menu_container">
            <div class="envio">
                <i class="fa-solid fa-location-dot"></i>
                <p id="nombre_envio">Enviar a Santiago</p>
                <p id="direccion_envio">Chivilcoy 2745</p>
            </div>
            <ul class="menu">
                <li>Categorias</li>
                <li>Ofertas</li>
                <li>Historial</li>
                <li>Supermercado</li>
                <li>Moda</li>
                <li>Vender</li>
                <li>Ayuda</li>
            </ul>
            <div class="menu_user">
                <ul>
                    <li><i  class="fa-regular fa-circle-user"></i> Santiago <i class="fa-solid fa-chevron-down"></i></li>
                    <li>Mis compras</li>
                    <li>Favoritos <i class="fa-solid fa-chevron-down"></i></li>
                </ul>
                <i class="fa-regular fa-bell"></i>
            <i class="fa-solid fa-cart-shopping"></i>
            </div>
            
        </div>    
    </div>
</template>

<script>
export default {
    
}
</script>
<style scoped>
.navbar{
    width: 100%;
    background-color: #FFF159;
    min-height: 100px;
    display: flex;
    flex-direction: column;
    font-family: Arial, Helvetica, sans-serif;
    user-select: none;
}
#logo{
    width: 140px;
    cursor: pointer;
}
#disney_promo{
    width: 350px;
    cursor: pointer;
}



/* container abajo */


.envio_menu_container{
    display: flex;
    align-items: center;
/*     border: 1px solid red; */
    justify-content: center;
    gap: 5%;
}
.envio{
    position: relative;
    width: 140px;
    height: 45px;
    border-radius: 3px;
    padding: 2px;
}
.envio:hover{
   border: 1px solid rgb(195, 195, 186); 
}
#nombre_envio{
    position: absolute;
    top: 5px;
    right: 8px;
    font-size: 12px;
    color:  rgb(149, 149, 139);
}
#direccion_envio{
    position: absolute;
    right: 8px;
    top: 20px;
        color:  rgb(56, 56, 52);
        font-size: 14px;
}
.envio i{
    font-size: 25px;
}
.search_bar_logo{
    display: flex;
    align-items: center;
    height: 55px;
justify-content: center;
gap: 50px;
}
.searchbar{
    width:560px;
    height: 40px;
    background-color: white;
    box-shadow: 1px 1px 2px 0px rgb(185, 185, 185);
    position: relative;
}
.searchbar input{
    height: 100%;
    border: none;
    width: 100%;
    padding-left: 20px;
    color: rgb(202, 202, 202);
    font-size: 16px;
}
.searchbar input:focus{
    outline: none;
}
.searchbar i{
    color: grey;
    position: absolute;
    right: 10px;
    top: 10px;
    font-size: 16px;
    font-weight: bold;
    
}
#barra{
color: rgb(230, 230, 230);   
position: absolute;
right: 35px;
font-size: 30px;
}   
.menu{
    display: flex;
    list-style-type: none;  
    font-size: 14px;  
}
.menu li {
    margin-left: 20px;
    color: rgb(108, 108, 108);
}
/* Menu User */
.menu_user{
    margin-left: 20px;
    display: flex;
    gap: 15px;
}
.menu_user ul{
    display: flex;
    align-items: end;
    list-style-type: none;
    font-size: 13px;
    gap: 10px;
    color: rgb(108, 108, 108);
}
.fa-circle-user{
    font-size: 22px;
    color: rgb(88, 88, 88);
}
.fa-chevron-down{
    color: rgb(211, 211, 211);
    cursor: pointer;
}
.fa-bell,.fa-cart-shopping{
font-size: 20px;
color: rgb(36, 36, 36);
margin-left: 10px;
}
</style>