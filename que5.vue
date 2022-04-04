<template>
    <div id="class">
        <h2>error handling</h2>
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
computed:{

errorshandling(test) {
    try{
test = val * 45;
console.log("test",val);
    }
    catch{
        console.log("ds");
    }
}
}
}

</script>
