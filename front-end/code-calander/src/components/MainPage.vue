<template>
  <!-- everything goes inside of these divs -->
  <div class="giant-container" style="border: 1px solid red; height: 100vh;">
    <div class="menu">
      <img src="../media/code_calanderV1.png" width="20%" style="float: left; margin:30px; margin-top:0px; "/>
      <ul style="margin-right:40px">
        <li>About</li>
        <li>Contact</li>
      </ul>
    </div >
    <div style="margin:40px; margin-top:100px;">
      <p>Maybe something written here about clicking on the day to show information?</p>
    </div>
  
    <div class="calendar">
<h1>Calendar goes here</h1>
    </div>

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
  float: right;
margin:30px;
}
.menu{
  margin-top: 30px;
}
.calendar{
margin:150px;
  text-align: center;
  border: 1px solid;
  border-color: green
}
</style>
