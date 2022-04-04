<template>
    <div id="class">
        Firstname: <input type = "text" v-model = "firstname" /> <br/><br/>
        Lastname: <input type = "text" v-model = "lastname"/> <br/><br/>

         <h1>My name is {{firstname}} {{lastname}}</h1>
         <!--<h1>Using computed method : {{getfullname}}</h1>-->
      </div>
</template>
<script>
export default{
name:"QuE10",
data(){
    return{
      firstname :"",
      lastname :"",
    }
},
    computed:{
getfullname : function(){
         return this.firstname +" "+ this.lastname;
}
}
}
</script>
