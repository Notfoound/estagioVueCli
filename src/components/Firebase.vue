<script>
import firebase from 'firebase'

var config = {
    apiKey: "AIzaSyDfVoxXZ99_WZLk_sJz9G3GnCdEOBs-gJc",
    authDomain: "estagio-2018.firebaseapp.com",
    databaseURL: "https://estagio-2018.firebaseio.com",
    projectId: "estagio-2018",
    storageBucket: "estagio-2018.appspot.com",
    messagingSenderId: "751571535533"
}
var app = firebase.initializeApp(config);
var db = app.database()
var listRef = db.ref('users')

export default {
    name: 'Firebase',
    firebase: {
      listRef: listRef
    }
}
</script>

<style>

</style>
