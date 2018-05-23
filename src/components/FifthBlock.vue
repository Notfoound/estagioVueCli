<template>
    <div class="content-6">
        <div class="lg-container">
            <h2>Autenticação</h2>
            <p>Preencha os campos abaixo para se autenticar</p>
            <form>
                <label>E-mail</label>
                <input type="text" class="form-control" id="formUser"  v-bind="email" name="email" placeholder="email" required/>
                <label>Senha</label>
                <input type="password" class="form-control" id="" name="pass"  v-bind="pass" placeholder="Password" required />
                <input type="submit" id="bt-sub" v-on:click="login()" class="bt-ticket" value="SUBMIT" />
            </form>
        </div>
    </div>
</template>

<script>

import firebase from 'firebase'

export default {
    name: 'Fifth',
    data() {
        return{
            email: '',
            pass: '',
        }
    },
    methods: {
        login(){
            firebase.auth().signInWithEmailAndPassword(this.email, this.pass)
            .then((result) => {
                alert("Bem vindo!" + result)
            })
            .catch((error) =>{
                alert("Falha na autenticação!" + error.code)
            });
        },
        create(){
            firebase.auth().createUserWithEmailAndPassword(this.email, this.pass)
            .then((result) => {
                alert("Bem vindo!" + result)
            })
            .catch((error) =>{
                alert("Falha na autenticação!" + error.code)
            });
        }
    }
}
</script>

<style scoped>
.content-6{
    height: 100%;
    width: 100%;
    display:flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-color: white;
}
.lg-container{
    padding: 5% 30px 5% 30px;
    display: table;
    width: 30%;
    margin: 30px;
}
h2{
    font-size: 30px;
    text-transform: uppercase;
    color: #333;
}
.form-control{
    border: none;
    padding: 5px;
    color: #bdbdbd;
    font-size: 18px;
    width: 100%;
    border: 1.5px solid #bdbdbd;
    border-radius: 4px;
    margin-bottom: 10px;
    text-transform: lowercase;
}
.bt-ticket{
    margin-top: 30px;
    padding: 10px 20px 10px 20px;
    background-color: #d4d41b;
    color: #015da0;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    font-size: 16px;
    text-transform: uppercase;
}
.bt-ticket:hover{
    -webkit-transition: all 0.3s ease-in-out;
    -moz-transition: all 0.3s ease-in-out;
    -o-transition: all 0.3s ease-in-out;
    transition: all 0.3s ease-in-out;
    background-color: #015da0;
    color: white;
}

</style>
