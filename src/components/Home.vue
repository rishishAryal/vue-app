<template>
<h1>Home Components </h1>
<h1>Email is {{ email }} </h1>
<h1>email is {{ getData().email }} </h1>
</template>

<script>
export default {
    name: 'Home',
    data(){
        return {
            email:'risharyal5@gmail.com'
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
        }
    }
}
</script>
<style scoped>
h1{
    color: rgb(9, 124, 85);
}
</style>