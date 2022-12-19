<template class ="teste">
    <div>
        <h1>Podcastr</h1>
        <p id="texto"> O melhor para você ouvir, sempre</p>
        <p id="data">data, data2</p>
    </div>    
</template>

<style scoped>
div{
    position: absolute;
    width: 1016px;
    height: 104px;
    background-color:  #ff0000;
    display:flex;
    align-items: center;
    justify-content: space-between;
}
h1{
    margin-left: 58px;
    margin-top: 11px;
    order: 1;
    
}
p{
    color:  #808080;
    font-family: 'Roboto';
}
#texto{
    /* background-color: black; */
    
    font-size: 14px;
    margin-left: 130px;
    order: 2;
    flex-grow: 2;
    
}
#data{
    margin-right:64px ;
    order: 3;
}

</style>