<template>
  <div class="kk">
    <h1>Hello!! I am the parent....</h1>
    <h2>Name is: {{childname}}</h2>
    <Child :childname="childname" :chg="change"></Child>
  </div>
</template>

<script>
import child from './child';
export default {
  components:{
    Child : child
  },
  data: function(){
    return{
      childname : "kartik"
    }
  },
  methods:{
    change(){
      console.log("Parenting executing...");
      this.childname="Aishwary";
    }
  }
}
</script>

<style scoped>
  h1{
    color: red;
  }
  div{
    margin: 3rem;
  }
  .kk{
    background-color: cornsilk;
    padding: 3rem;
  }
</style>>

</style>
