<template>
    <div id="class">
        <h2>error handling</h2>
        <button @click="errorshandling()">catch</button>
    </div>
</template>
<script>
export default{

name:"HellO",
data(){

return{
    test:" "
}
},
methods:{
errorshandling() {
    try{
this.test = this.val * 45;
console.log("test",this.val);
    }
    catch{
        console.log("error");
    }
}
}
}

</script>
