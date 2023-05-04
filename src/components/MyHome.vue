<template>
<h1>Home Components </h1>
<h1>Email is {{ email }} </h1>
<h1>email is {{ getData().email }} </h1>
  <h1 v-on:mousemove="getConsole()" style="background-color: aqua">Please dontHover here</h1>
<button v-on:click="increaseCounter()">click here to increase count</button>
<button v-on:dblclick="test('double clicked')">double click</button>
<button v-on:click="decreaseCounter()">click here to decrease count</button>
  <h1>Counter: {{count}} </h1>
</template>


<script>
export default {
    name: 'MyHome',

    data(){
        return {
            email:'risharyal5@gmail.com',
             count:0
        }
    },
    methods:{
        getName(){
            return "Rishish Aryal"
        },
        getData(){
            return  {
                name:"rish",
                age:20,
                email:this.email
            }
        },
        test(data){
            alert(data)
        },
      getConsole(){
         this.count=0

        // console.log("hello world")
      },
      increaseCounter(){
          this.count+=1;
      },
      decreaseCounter(){
          this.count-=1;
      }

    }
}
</script>
<style scoped>
h1{
    color: rgb(9, 124, 85);
}

</style>
