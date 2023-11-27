<template>
  <div class="dropdown">
  <button @click="show = !show" class="btn btn-secondary dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
    {{selectedOption}}
  </button>
  <ul  :class="show?'dropdown-menu show' : 'dropdown-menu'" >
    <DropdownItem v-for="option in options" :key="option" @select="handleClick(option)" :option="option"></DropdownItem>
  </ul>
</div>
</template>
<!---->
<script>
import DropdownItem from './DropdownItem.vue';

export default {
    name: "AppDropdown",
    data() {
        return {
            options: ["Option 1", "Option 2", "Option 3"],
            selectedOption: "Select an option",
            show: false
        };
    },
    methods: {
        handleClick(option) {
            this.selectedOption = option;
            this.show = false;
        }
    },
    components: { DropdownItem }
};
</script>

<style >
</style>
