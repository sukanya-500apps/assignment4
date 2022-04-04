<template>
    <div>
        <h1>spread operator</h1>
        <button @click="fun()">click</button>
    </div>
</template>
<script>
export default{
    name:"SpreaD",
    data(){
        return{
         array:[1,2,3,7,8,6,9,10],
         array1:[4,5]
       
        }
    },
methods:
    {
     fun(){
const array=[1,2,3,7,8,...this.array1,9,10]
console.log(array);
        }
    }
   
}
</script>

