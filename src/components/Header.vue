<template class ="teste">
    <div>
        <img src="../assets/Logo.png" alt="PODCASTR">
        <p id="texto"> O melhor para você ouvir, sempre</p>
        <p id="data">data, data2</p>
    </div>    
</template>

<style scoped>
div{
    height: 100%;
    width: 100%; 
    background-color:  #ffffff;
    display:flex;
    align-items: center;
    justify-content: space-between;
}
img{
    margin-left: 58px;
    margin-bottom: 32px;
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