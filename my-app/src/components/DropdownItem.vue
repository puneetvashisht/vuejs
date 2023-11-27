<template>
 <li><a @click="handleClick(option)" class="dropdown-item" href="#">{{option}}</a></li>
</template>

<script>
export default {
  name: 'DropdownItem',
  // Component properties and methods go here
  props: {
    option: String,
  },
  methods: {
    handleClick(option) {
        console.log('In child component', option);
      this.$emit('select', option);
    }
  },
}
</script>

<style >

</style>
