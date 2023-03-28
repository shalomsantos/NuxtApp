<template>
    <header class="shadow-sm bg-white">
        <nav>
            <ul id="ul-Principal">
                <li class="li-p"><a href="">Home</a></li>           
                <li class="li-p">
                    <a href="javascript://" class="bt1">
                        Cadastro                    
                    </a>
                    <ul class="ul-cadastro">
                        <li><a href="/views/Cadastro_ClientePf.html">Clientes</a></li>                    
                        <li><a href="">Produtos</a></li>
                        <li><a href="">Produtos Grupos</a></li>
                        <li><a href="">Estoque</a></li>
                    </ul>
                </li>
                <li class="li-p">
                    <a href="javascript://" class="bt2">
                        Estoque                    
                    </a>
                    <ul class="ul-consultas">
                        <li><a href="">Consultar</a></li>
                    </ul>
                </li>
                <li class="li-p">
                    <a href="javascript://" class="bt3">
                        Promissórias                    
                    </a>
                    <ul class="ul-promissoria">
                        <li><a href="">Confi-Promissoria</a></li>
                    </ul>
                </li>
                <li class="li-p">
                    <a href="javascript://" class="bt4">
                        Rotinas                   
                    </a>
                    <ul class="ul-rotinas">
                        <li><a href="">Pedidos</a></li>
                        <li><a href="">Contas a Receber</a></li>
                        <li><a href="">Recibos</a></li>
                    </ul>
                </li>
                <li class="li-p">
                    <a href="javascript://" class="bt5">
                        Alterar Senha                   
                    </a>
                    <ul class="ul-senha">
                        <li><a href="">Criar Senha</a></li>
                        <li><a href="">Permisão de Senha</a></li>
                    </ul>
                </li>
                <li class="li-p"><a href="/views/Login-Rens.html">Voltar</a></li>  
            </ul>
        </nav>
    </header>
    <div class="container mx-auto p-4">
        <slot/>
    </div>
</template>

<script lang="js" setup>
</script>

<style scoped>
*{
    padding: 0px;
    margin: 0px;
}
body {
    font-family: arial;
    background-image: linear-gradient(to right, rgb(35, 189, 265), rgb(55, 218, 63));
    background-size: 100%;    
}
ul{
    list-style: none;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
}
a{
    text-decoration: none;
    color: white;    
    display: block;
    padding: 0px 20px;
}
a:hover{
    background-color: rgba(255,255,255,.3);

}
nav{
    background-color: rgb(0, 113, 241);
    height: 50px;
}
ul#ul-Principal{
    background-color:  rgb(0, 113, 241);;
    width: 90%;
    margin: auto;
}
.li-p{
    line-height: 50px;
    float: left;
   
}
ul li ul li{
    background-color: rgb(0, 113, 241);
    font-family: monospace 
   
}

.ul-cadastro, .ul-consultas, .ul-promissoria, .ul-rotinas, .ul-senha{
    display: none;
}
@media screen and (max-width: 768px) {
    section, aside {
        width: 100%;
        padding: 0;
    }
    
}
@media screen and (max-width: 600px) {
    nav li{
        float: none;
        text-align: center;
        width: 100%;
    }
}
</style>