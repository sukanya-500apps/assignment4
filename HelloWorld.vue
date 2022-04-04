<template>
  <div class="hello">
    <sukanya :message="message" />
  </div>
</template>

<script>
import sukanya from './parent.vue'
export default {
  name: 'HelloWorld',
components:{
  sukanya
},
data(){
return{
message:"welcome",
}
}
}
</script>

