<template>
<footer>
    <div class="center-al-row">
        <p>Desenvolvido por {{ autor }}</p>
        <p>{{ date }}</p>
        <p>Versão {{ version }}</p>
    </div> 
</footer>   
</template>

<script>
export default {
    name: 'Footer',
    data(){
        return{
            autor: 'Matheus Henrique',
            date: '23/05/2018',
            version: '1.0'
        }
    }
}
</script>

<style scoped>
.center-al-row{
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
}
footer{
    width: 100%;
    padding: 3% 0 3% 0;
    background-color: #00142a;
    color: white;
    font-family: 'Roboto Condensed Regular';
    text-transform: uppercase;
    font-size: 14px;
}
footer p{
    margin: 15px;
}

</style>
