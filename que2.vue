<template>
    <div id ="class">
        <form id="demo">
  <p>{{msg}}</p>
  <p>{{msg.length}}</p>
    <input type="text" name="message" v-model="msg">
        </form>
    </div>
</template>
<script>
export default{
    name:"QuE2",
    data(){
return{
msg:""
}
    }
}
</script>
