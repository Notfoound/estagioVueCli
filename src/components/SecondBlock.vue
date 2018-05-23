<template>
<div class="content-2">
    <div class="align-main">
    <div class="bc02-al-title">
        <div class="bc02-logo">
            <img id="logo-team" src="/static/emblem-real-madrid.svg" >
        </div>
        <div class="center-al-row"><p>{{ name }}</p></div>
    </div>
    <div class="bc02-al-infoStadium">
        <label>Estádio</label>
        <p>{{ stadium }}</p>
    </div>
    <div class="bc02-abs">
        <div class="align-section">
        <p class="text">{{ history }}</p>
        </div>
        <div class="align-section">
            <div class="bc02-abs-img center-al-row">
                <img class="img-resize-box" src="/static/history-real-madrid-01.jpg">
            </div>
            <div class="bc02-abs-img2 center-al-row">
                <img class="img-resize-box" src="/static/history-real-madrid-02.jpg">
            </div>
        </div>
        <div class="align-section">
            <div class="bc02-abs-stadium">
                <img class="mainImg-resize-box" src="/static/history-real-madrid-stadium.jpg" >
            </div> 
        </div>
    </div>
    </div>
    </div>
</template>

<script>
export default {
    name: 'Second',
    data(){
        return{
            name: 'Real Madrid Club Fútbol',
            stadium: 'Santiago Bernabéu',
            history: 'A história do Real Madrid Club de Fútbol começa em 1902 em Madri, capital da Espanha, quando funda a equipe que seria o futuro conjunto merengue.  O Real Madrid é um dos clubes de futebol com mais renome mundial, em 11 de dezembro de 2000, em sua festa anual, a FIFA lhe concedeu o título de Melhor Clube do Século XX aos "merengues". Em suas vitrines conta com trinta e três campeonatos de Liga, dezenove Copas do Rei, nove supercopas da Espanha, fazendo-lhe o conjunto mais vencedor de seu país, com doze Liga dos campeões, duas copas da UEFA, três Supercopa da Europa, três Copas Intercontinentais, e dois mundiais da FIFA.' 

        }
    }
}
</script>

<style scoped>
.align-main{
    width: 75%;
    margin: 0 auto;
    height: 100%;
    max-width: 1400px;
    padding: 0 0.5% 0 0.5%;
    /*background-color: rgba(255, 255, 255, 0.2);*/
}
.align-section{
    margin: 0 0.5% 0 0.5%;
    width: 32.33%;
    height: 100%;
    position: relative;
    float: left;
}

.center-al-column{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
.center-al-row{
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
}
.content-2{
    height: 100%;
    width: 100%;
    display: table;
    background-color: rgba(255, 255, 255, 1);
}
.bc02-al-title{
    display: table;
    float: left;
    margin-top: 50px;
}
.bc02-logo{
    height: 80px;
    width: 80px;
    float: left;
}
.bc02-al-title p{
    display: inline;
    font-size: 30px;
}
.bc02-al-infoStadium{
    display: table;
    clear: both;
    float: right;
    margin-right: 0.5%;
}
.bc02-al-infoStadium label{
    font-size: 18px;
    margin: 0;
    float: right;
}
.bc02-al-infoStadium p{
    font-size: 24px;
    margin: 0;
    clear: both;
    text-align: right;
}
.bc02-abs{
    clear: both;
    width: 100%;
    height: 480px; 
    margin-bottom: 10%;
}
.bc02-abs-img{
    padding-bottom: 1.5%;
    height: 50%;
    width: 100%;
    overflow: hidden;
    float: left;
}
.bc02-abs-img2{
    padding-top: 1.5%;
    height: 50%;
    width: 100%;
    overflow: hidden;
    float: left;
}
.bc02-abs-stadium{
    height: 100%;
    width: 100%;
    overflow: hidden;
}
.img-resize-box{
    height: 100%;
    cursor: pointer;
}
.mainImg-resize-box{
    height: 100%;
    cursor: pointer;
}

</style>
