<template>
  <div>
    <h2>Vue Js Dropdown</h2>
    <select name="users" @change="onChange($event)" class="form-select form-control">
        <option>status</option>
        <option @click="open()" value="open">open</option>
        {{opendata}}
        <option @click="closed()" value="closed">closed</option>
        {{closeddata}}
        <option  @click="pending()" value="pending">pending</option>
        {{pendingdata1}}<br> {{pendingdata2}}
        <p>{{result}}</p>
</select>
    
  </div>
</template>
 
<script>
export default {
  name: "App",
  data() {

    return {
 users:[
{email: "Eliseo@gardner.biz",id: 1,name: "id labore ex et quamlaborum",status:"open"},
 {email: "Jayne_Kuhic@sydney.com",id: 2,name: "quovero reiciendis velit similiqueearum",status:"pending"},
  {email: "Nikita@garfield.biz",id: 3,name:"odioadipisci rerum autanimi",status:"closed"}, 
  {email: "Lew@alysha.tv",id: 4,name: "alias odio sit",status:"pending"}
],
result:"",
opendata:"",
closeddata:"",
pendingdata1:"",
pendingdata2:"",
          }
    },
    methods:{
        open(){
             this.opendata = this.users[0];
             console.log(this.opendata);
        },
        closed(){
            this.closeddata = this.users[2];
            console.log(this.closeddata);
        },
        pending(){
            this.pendingdata1 = this.users[1];
            this.pendingdata2 = this.users[3];
            console.log(this.pendingdata1);
            console.log(this.pendingdata2);
        },
        
    }
}
</script>