<template>
    <div class="content-5">
        <div class="align-main">
            <div class="bc05-header center-al-column">
                <h2>Principais Jogadores</h2>
                <p>{{ nameHome }}</p>
                <span>X</span> 
                <p>{{ nameAway }}</p>
            </div>
            <div class="bc05-content">
                <div class="align-section">
                    <div class="bc05-content-group">
                        <div class="bc05-content-player ronaldo" ></div>
                        <div class="bc05-content-info" >
                            <div class="bc05-info-personal">
                                <p>Cristiano</p><br />
                                <span>Ronaldo</span>
                                <img src="/static/Flag_of_Portugal.svg" class="bc05-flags">
                            </div>
                            <div class="bc05-info-stats">
                                <div class="bc05-stats-side">
                                    <div class="bc05-stats-info">
                                        <label>Velocidade Máxima</label><br />
                                        <p>31 KM/h</p>
                                    </div>
                                    <div class="bc05-stats-info">
                                        <label>Assistências</label>
                                        <p>2</p>
                                    </div>
                                    <div class="bc05-stats-info">
                                        <label>Jogos</label>
                                        <p>12</p>
                                    </div>
                                </div>
                                <div class="bc05-stats-side">
                                    <div class="bc05-stats-info">
                                        <label>Precisão dos passes</label>
                                        <p>80%</p>
                                    </div>
                                    <div class="bc05-stats-info">
                                        <label>Ocasiões</label>
                                        <p>79</p>
                                    </div>
                                    <div class="bc05-stats-info">
                                        <label>Gols</label>
                                        <p>15</p>
                                    </div>
                                </div>    
                            </div>
                        </div>
                    </div>
                </div>
                <div class="align-section">
                    <div class="bc05-content-group">
                        <div class="bc05-content-player salah" ></div>
                        <div class="bc05-content-info" >
                        <div class="bc05-info-personal">
                                <p>Mohamed</p><br />
                                <span>Salah</span>
                                <img src="/static/Flag_of_Egypt.svg" class="bc05-flags">
                            </div>
                        
                            <div class="bc05-info-stats">
                                <div class="bc05-stats-side">
                                    <div class="bc05-stats-info">
                                        <label>Velocidade Máxima</label><br />
                                        <p>33 KM/h</p>
                                    </div>
                                    <div class="bc05-stats-info">
                                        <label>Assistências</label>
                                        <p>4</p>
                                    </div>
                                    <div class="bc05-stats-info">
                                        <label>Jogos</label>
                                        <p>12</p>
                                    </div>
                                </div>
                                <div class="bc05-stats-side">
                                    <div class="bc05-stats-info">
                                        <label>Precisão dos passes</label>
                                        <p>79%</p>
                                    </div>
                                    <div class="bc05-stats-info">
                                        <label>Ocasiões</label>
                                        <p>41</p>
                                    </div>
                                    <div class="bc05-stats-info">
                                        <label>Gols</label>
                                        <p>10</p>
                                    </div>
                                </div>    
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Fourth',
    data(){
        return{
            nameHome: 'Real Madrid',
            nameAway: 'Liverpool'
        }
    }
}
</script>

<style scoped>
.content-5{
    height: 100%;
    width: 100%;
    display: table;
    background-image: url("/static/bg-04.jpg");
    background-repeat: no-repeat;
    background-size: cover;
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
h2{
    font-size: 30px;
    text-transform: uppercase;
    font-family: 'Roboto Condensed Bold';
    color: white;
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
.bc05-header{
    margin-top: 5%;
    width: 100%;
    height: 200px;
}
.bc05-header p {
    margin: 0;
    font-size: 24px;
    color: white;
    text-transform: uppercase; 
}
.bc05-header span{
    margin: 0;
    color: white;
}
.bc05-header h2{
    margin-bottom: 10px;
}
.bc05-content{
    height: 800px;
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
}
.bc05-content-group{
    height: 500px;
    width: 250px;
    margin: 0 auto;
    margin-bottom:  5%;
}
.bc05-content-player{
    height: 60%;
    width: 100%;
    float: left;
}
.bc05-content-info{
    height: 200px;
    width: 100%;
    display: table;
    float: left;
    background-color: aqua;
}
.ronaldo{
    background-image: url('/static/ronaldo.png');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}
.salah{
    background-image: url('/static/salah.png');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}
.bc05-info-personal{
    padding: 10px 0 10px 0;
    width: 100%;
    display: table;
    padding: 10px;
    float: left;
    position: relative;
    background-color: #015da0;
}
.bc05-info-personal p{
    font-size: 18px;
    margin: 0;
    float: right;
    color: white;
    text-transform: capitalize; 
}
.bc05-info-personal span{
    font-size: 24px;
    margin: 0;
    float: right;
    color: white;
    text-transform: uppercase; 
}
.bc05-info-stats{
    padding: 10px 0 10px 0;
    width: 100%;
    display: table;
    padding: 10px;
    float: left;
    background-color: white;
}
.bc05-flags{
    position: absolute;
    height: 30%;
    top: 40%;
    left: 10%;
}
.bc05-stats-side{
    width: 50%;
    display: table;
    float: left;
}
.bc05-stats-info{
    width: 100%;
    height: 100px;
    float: left;
}
.bc05-stats-info label{
    font-size: 12px;
    color: #6f6f6f;
    text-transform: uppercase; 
}
.bc05-stats-info p{
    font-size: 18px;
    color: #333;
    text-transform: uppercase; 
}
</style>
