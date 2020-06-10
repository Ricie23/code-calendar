<template>
  <!-- everything goes inside of these divs -->
  <div class="giant-container" style="border: 1px solid red; height: 100vh;">
      <h1>Hello Welcome to CodeCalendar.com!</h1>
      <p>All of our stuff should go between these template tags surrounding this code</p>
      <p>Styles for everything on this page can be added below in the style tag</p>
      <p>inside of the script below is where we can add variables and lifecycle hooks</p>
  </div> 
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
    color: green;
}
.giant-container {
    text-align: center;
}
</style>
