<template>
    <div class="fundo">
        <img src="../assets/Top.png" alt="TOCANDO AGORA" class="agora">
        <div class="player">
            <p>Selecione um<br>podcast para ouvir</p>
        </div>
        <div class="progress-bar">
            <span>00:00------------------------------00:00</span>
        </div>
        <div class="botoes">
            <button id="shuffle"></button>
            <button id="previous"></button>
            <button id="play"></button>
            <button id="next"></button>
            <button id="repeat"></button>
            
        </div>
    </div>
</template>

<style scoped>
.fundo{
 background-color: #8257E5;
 width: 424px;
 height: 820px;
 display: flex;
 flex-direction: column;
 align-items: center;
}
.agora{
    order: 1;
    margin-top: 5%;
    
}
.player{
    background:linear-gradient(#9164FA,#9164FA00);
    width: 296px;
    height: 346px;
    margin-top: 126px;
    margin-bottom: 126px;
    order: 2;
    border-radius: 24px;
    text-align: center;
    justify-content: center;
    border-style: dashed;
    border-color: #9F75FF;
    color:#ffffff ;
}
.player>p{
    margin-top: 50%; 
}
.progress-bar{
    order: 3;
    margin-bottom: 45px;
    font-size: 14px;
    color: #ffffff;
}
.botoes{
    order: 4;
    width: 256px;
    margin-bottom: 48px;
    margin-left: 0px;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    
}
button
{
  width: 24px;
  height: 24px;
  background-color:#8257E5 ;
  border: none;
}
#shuffle{
    background-image: url('../assets/shuffle.png');

}
#previous{
    background-image: url('../assets/play-previous.png');
}
#play{
    width: 64px;
    height: 64px;
    border-radius: 16px;
    background-color: #9164FA;
    background-image: url('../assets/play.png');
    background-repeat: no-repeat;
    background-position: center;
    background-size: 32px;

}
#next{
    background-image: url('../assets/play-next.png');
}
#repeat{
    background-image: url('../assets/repeat.png');
}
</style>