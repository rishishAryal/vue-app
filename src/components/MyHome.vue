<template>
<h1>Home Components </h1>
<h1>Email is {{ email }} </h1>
<h1>email is {{ getData().email }} </h1>
  <h1 v-on:mousemove="getConsole()" style="background-color: aqua">Please don't Hover  there is nothing to do</h1>
<button v-on:click="increaseCounter()">click here to increase count</button>
<button v-on:dblclick="multiplyByTwo()">double click
  to multiply the count value by 2</button>
<button v-on:click="decreaseCounter()">click here to decrease count</button>
  <h1>Counter: {{count}} </h1>
  <input type="text"  v-model="count"/>
</template>


<script>
export default {
    name: 'MyHome',

    data(){
        return {
            email:'risharyal5@gmail.com',
             count:0,


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
      multiplyByTwo(){
          this.count*=2;
      },
      getConsole(){


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
