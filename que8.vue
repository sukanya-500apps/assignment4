<template>
<div>
<p @click="func()">
p tag : kiran
</p>
<textarea id="id">
</textarea>
</div>
</template>
<script>
export default {
name: "QuE8",
data() {
return {
text: "",
};
},
methods: {
func() {
this.text= " " + document.getElementById("id").value;
document.write(this.text);
}
},
};
</script>



