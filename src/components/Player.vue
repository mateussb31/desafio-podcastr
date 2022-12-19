<template>
    <div class="fundo">
        <p class="agora">TOCANDO AGORA</p>
        <div class="player">
            <p>Selecione um<br>podcast para ouvir</p>
        </div>
        <div class="progress-bar">
            <span>00:00------------------------------00:00</span>
        </div>
        <div class="botoes">
            <button id="shuffle"></button>
            <button></button>
            <button></button>
            <button></button>
            <button></button>
            
        </div>
    </div>
</template>

<style scoped>
.fundo{
 background-color: #8257E5;
 width: 424px;
 height: 820px;
 right: 0;
 position: absolute;
 display: flex;
 flex-direction: column;
 align-items: center;
}
.agora{
    order: 1;
    margin-bottom: 126px;
}
.player{
    background:linear-gradient(#9164FA,#9164FA00);
    width: 296px;
    height: 346px;
    margin-bottom: 126px;
    order: 2;
    border-radius: 24px;
    text-align: center;
    align-items: center;
    justify-content: center;
    border-style: dashed;
    border-color: #9F75FF;
    color:#ffffff ;
}
.progress-bar{
    order: 3;
    margin-bottom: 45px;
    font-size: 14px;
    color: #ffffff;
}
.botoes{
    order: 4;
    margin-bottom: 48px;
}
#shuffle
{
  margin: 0 auto;
  top: 25%;
  position: relative;  
  width: 0;
  height: 0;
  border-style: solid;
  border-width: 2.5em 0 2.5em 5em;
  
  opacity: .75; 
}
</style>