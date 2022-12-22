<template>
<h2>Ultimos Lancçamentos</h2>
    <div class="secao">
        <div v-for="item in listaEpsodios.slice(-2)" class="lancamento">
            
            <img :src=item.thumbnail alt="Thumbnail podcast"/>
            <p id="Titulo">{{item.title}}</p>
            <p id="Nomes">{{item.members}}</p>
            <p id="Pequenos">{{item.published_at.split(' ')[0]}}</p>
            <p id="Pequenos">{{converteTempo(item.file.duration)}}</p>
            <button class="play"></button>
        </div>
    </div>

</template>

<script lang="ts">
import epsodes from "../assets/epsodes.json"
import {converteTempo} from "../utils/conversor.vue"
export default {
    data() {
        return {
            listaEpsodios: epsodes
        }
    },
    methods:{
        converteTempo,
    },
}
</script>

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
    font-size: 14px;
    line-height: 17px;
    max-width: 60%;
    max-height: 14%;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
}
img{
    margin: 20px;
    width: 96px;
    height: 96px;
    float: left;
    border-radius: 12px;
}
#Titulo{
    font-size: 16px;
    
    color: #494D4B;
    margin-top: 29px;
    margin-bottom: 0px;
    margin-left: 116px;
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