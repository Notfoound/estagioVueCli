<template>
    <div class="content-1">
        <div class="align-main">
        <div class="bc01-logo center-al-column">
            <img id="logo-uefa" src="static/emblem-uefa.svg" >
        </div>
        <div class="bc01-info">
            <div class="align-section">
                <div class="bc01-team-name center-al-column">
                    <h2>{{home}}</h2>
                </div>
                <div class="bc01-team-emblem center-al-column">
                    <img id="logo-team" alt="Real Madrid" src="static/emblem-real-madrid.svg">
                </div>
            </div>
            <div class="align-section" id="info-finals">
                <p>Final, Kyev 2018</p>
                <p>Sábado 26 de maio</p>
                <p>15:45</p>
            </div>
            <div class="align-section">
                <div class="bc01-team-emblem center-al-column">
                    <img id="logo-team" alt="Liverpool" src="/static/emblem-liverpool.svg">
                </div>
                <div class="bc01-team-name center-al-column" >
                    <h2>{{ visitor }}</h2>
                </div>
            </div>
        
        </div> 
    </div>
    </div>
</template>

<script>


export default {
    name: 'First',
    data(){
        return {
            home: "Real Madrid",
            visitor: "Liverpool"
        }
    }
}
</script>

<style scoped>
.content-1{
    height: 100vh;
    width: 100%;
    margin: 0;
    background-image: url("/static/bg-01.jpg");
    background-repeat: no-repeat;
    background-size: cover;
} 
html, body{ 
    margin: 0;
    width: 100%;
    height: 100%;
    min-width: 270px;
    font-size: 18px;
    color: #333;
}
body {
	overflow-x: hidden;
}
h2{
    font-size: 30px;
    text-transform: uppercase;
    color: white;
}
#info-finals p{
    font-size: 24px;
    color: white;
    text-align: center;
    line-height: 13px;
    text-transform: uppercase;
}
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
.bc01-info{
    width: 100%;
    height: 14%;
    display: table;
    top: 30%;
    position: relative;
}
.bc01-logo{
    width: 32.33%;
    margin: 0 auto;
    height: 30%;
    position: relative;
    top: 15%;
}
#logo-uefa{
    width: 70%;
}
#logo-team{
    width: 70%;
}
.bc01-team-name{
    width: 70%;
    height: 100%;
    float:left;
}
.bc01-team-emblem{
    width: 30%;
    height: 100%;
    float: left; 
}
#bt-bc-01{
    position: absolute;
    top: 90%;
    left: 50%;
    transform: translate(-50%, 60%);
}

</style>
