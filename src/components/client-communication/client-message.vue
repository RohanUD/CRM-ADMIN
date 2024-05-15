<template>
  <div :class="{'dark': backgroundChange}">
    <h5>{{ title }}</h5>
    {{ text }}
  </div>
</template>

<script>
export default {
    props : {
        text : String,
        title : String,
        backgroundChange : Boolean
    }
}
</script>

<style scoped>
.message {
  background: #e7e7e7;
  border-radius: 10px;
  padding: 1rem;
  width: fit-content;
}

.message.dark {
  background: #e9eaf6;
}

h5 {
  margin: 0 0 .5rem 0;
}
</style>