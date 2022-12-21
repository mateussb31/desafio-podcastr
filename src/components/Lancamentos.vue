<template>
<h2>Ultimos Lancçamentos</h2>
    <div class="secao">
        
        <div class="lancamento">
            <img src="" alt="Imagem"/>
            <p id="Titulo">Exemplo Exemplo Exemplp</p>
            <p id="Nomes">Nomes </p>
            <p id="Pequenos">data</p>
            <p id="Pequenos">tempo</p>
            <button class="play"></button>
        </div>
        <div class="lancamento">
            <img src="" alt="Imagem"/>
            <p id="Titulo">Exemplo Exemplo Exemplp</p>
            <p id="Nomes">Nomes </p>
            <p id="Pequenos">data</p>
            <p id="Pequenos">tempo</p>
            <button class="play"></button>
        </div>
    </div>

</template>

<style scoped>
h2{
margin-left: 64px;
margin-bottom: 24px;
}

.secao{
    display: flex;
    justify-content: space-around;  
}
.lancamento{
    display: inline;
    width: 432px;
    height: 136px;
    border-radius: 24px;
    border: 1px;
    border-color: #E6E8EB;
    background-color: #FFFFFF;
}
.lancamento >p{
    color: #494D4B;
    font-size: 16px;
}
.lancamento >p{
    font-size: 14px;
    line-height: 17px;
    
}
img{
    margin: 20px;
    width: 96px;
    height: 96px;
    float: left;
}
#Titulo{
    color: #494D4B;
    margin-top: 29px;
    margin-bottom: 0px;

}
#Nomes{
    color: #808080;
    margin-top:8px ;
    margin-bottom: 16px;
}
#Pequenos{
    color: #808080;
    display: inline;
    margin-right: 20px;
}
.play{
    background-image: url('../assets/play.png');
    display: inline;
    background-position: center;
    float: right;
    width: 40px;
    height: 40px;
    margin-right: 30px;
    border-radius: 10px;
    border: 1px;
    border-color: #E6E8EB;
    background-color: #808080;
}
</style>