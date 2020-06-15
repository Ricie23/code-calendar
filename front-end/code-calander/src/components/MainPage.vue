<template>
  <!-- everything goes inside of these divs -->
  <div class="giant-container" style="border: 1px solid red; height: 100vh;">
    <div class="menu">
      <img src="../media/code_calanderV1.png" width="20%" style="float: left; margin:30px; margin-top:0px; "/>
      <ul style="margin-right:40px">
        <li>Contact</li>
        <li>About</li>
      </ul>
    </div >
    <div style="margin:40px; margin-top:100px;">
      <p>Maybe something written here about clicking on the day to show information?</p>
    </div>
  
    <div class="calendar">
      <h1>Calendar goes here</h1>
        <table id="calendar">
            <thead>
              <tr>
                <th>Sun</th>
                <th>Mon</th>
                <th>Tue</th>
                <th>Wed</th>
                <th>Thu</th>
                <th>Fri</th>
                <th>Sat</th>
              </tr>
            </thead>
            <tbody id="calendar-body">
                      <calendar></calendar>

            </tbody>
        </table>
        <div class="form-inline">

            <button class="btn btn-outline-primary col-sm-6" id="previous" onclick="previous()">Previous</button>

            <button class="btn btn-outline-primary col-sm-6" id="next" onclick="next()">Next</button>
        </div>
        <br/>
        <form class="form-inline">
            <label class="lead mr-2 ml-2" for="month">Jump To: </label>
            <select class="form-control col-sm-4" name="month" id="month" onchange="jump()">
                <option value=0>Jan</option>
                <option value=1>Feb</option>
                <option value=2>Mar</option>
                <option value=3>Apr</option>
                <option value=4>May</option>
                <option value=5>Jun</option>
                <option value=6>Jul</option>
                <option value=7>Aug</option>
                <option value=8>Sep</option>
                <option value=9>Oct</option>
                <option value=10>Nov</option>
                <option value=11>Dec</option>
            </select>
        </form>
    </div>

  </div>  
</template>
<script>
  import Calendar from './Calendar.js'
  export default {
    name: 'HelloWorld',
    props: {
      msg: String
    },
    Calendar:'calendar',
    
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
