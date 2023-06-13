<template>
<h1>from new component file named MyNewComponent.vue</h1>
  <h3>Technology</h3>
  <label for="java">Java</label>
  <input type="checkbox" value="java" v-model="technology" id="java">
  <br>
  <label for="php">php</label>
  <input type="checkbox" value="php" v-model="technology" id="php">
  <br>
  <label for="node">node</label>
  <input type="checkbox" value="node" v-model="technology" id="node">
  <br>
  <label for="javascript">javascript</label>
  <input type="checkbox" value="javascript" v-model="technology" id="javascript">
  <br>
  <h3>Who I am</h3>
  <label for="student">Student</label>
  <input type="radio" value="student" name="profession"  v-model="who" id="student">
  <label for="developer">Developer</label>
  <input type="radio" value="developer" v-model="who"  name="profession" id="developer">
  <h3>Selected Technology: {{technology}} </h3>
  <h3>I am a :  {{who}}</h3>
<h1>Topic :If else condition:</h1>
  <h1 v-if="show">If else condition</h1>
  <button v-on:click="showOrHide" >{{ text}}</button>

</template>
<script>

export default {
  name: 'MyNewComponent',

  data(){
    return {
      technology:[],
      who:null,
      show:true,
      text:"click here"
    }
  },
  methods: {

showOrHide(){

    this.show=!this.show;
if(this.show==true){

  this.text="Click here to hide something"

}
else{

  this.text="Click here to show something"
}
}
  }
}


</script>

<style>

</style>
