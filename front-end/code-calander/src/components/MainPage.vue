<template>
  <!-- everything goes inside of these divs -->
  <div class="giant-container" style="border: 1px solid red; height: 100vh;">
    <div class="menu">
      <img src="../media/code_calanderV1.png" width="20%" style="float: left; margin:30px; margin-top:0px; "/>
      <ul>
        <li>About</li>
        <li>Contact</li>
      </ul>
    </div >
    <p>Styles for everything on this page can be added below in the style tag</p>
  </div>  
</template>
<script>
  
  export default {
    name: 'HelloWorld',
    props: {
      msg: String
    },
    data() {
       return{
       
       }
    },
    methods:{

    }
  }
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1{
  color: green;
}
.giant-container{
  text-align: center;
}
.menu li{
  display: inline; 
  text-decoration: none;
margin:30px;
}
.menu{
  margin-top: 30px;
}
</style>
