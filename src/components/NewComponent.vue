<template>
  <h1 class="">from new component file named NewComponent.vue</h1>
  <div class="flex flex-column width-fifty column-gap">
    <input v-model="email" placeholder="emter email" class="padding-y padding-x" type="text"/>
    <input v-model="password" placeholder="enter password" class="padding-y padding-x" type="password"/>
    <button v-on:click="getData()"
      type="button"
      class="bg-red-dark text-light
      padding-x padding-y
      font-size-medium">
      click here to get values
    </button>
  </div>
</template>


<script>

export default {
  name: 'NewComponent',

  data() {
    return {
      email: null,
      password: null
    }
  },
  methods: {
    getData() {
console.log(`email is ${this.email} and password is ${this.password}`)

      this.password=''
    }
  }
}

</script>

<style>
.margin-left {
  margin-left: 10px;
}

.text-light {
  color: white;
}

.bg-red-dark {
  background-color: darkred;
}

.padding-x {
  padding-left: 15px;
  padding-right: 15px;
}

.padding-y {
  padding-top: 5px;
  padding-bottom: 5px;
}

.font-size-medium {
  font-size: 20px;
}

.flex {
  display: flex;
}

.flex-column {
  flex-direction: column;
}

.column-gap {
  gap: 10px;
}

.width-fifty {
  width: 50%;
}
</style>
