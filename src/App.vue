<template>
  <AddUrl @add="add"/>
</template>

<script>
import AddUrl from './components/AddUrl.vue'

export default {
  name: 'App',
  components: {
    AddUrl
  },
  methods: {
    add(value) {
      console.log("App: Got emitted value from child (addUrl): " +value);
    }
  }
}
</script>

<style>

</style>
