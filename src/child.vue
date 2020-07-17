<template>
  <div>
    <h1>Hello!! I am the child....</h1>
    <h2>my name is {{childname}} .</h2>
    <button @click="changename">Change name</button>
  </div>
</template>

<script>
export default {
  props: ["childname","chg"],
  methods:{
      changename(){
          this.chg();
      }
  }
}
</script>

<style scoped>
    h1{
        color: blue;
    }
    div{
        background-color: burlywood;
        padding: 2rem;
    }
</style>>

