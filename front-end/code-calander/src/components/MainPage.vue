<template>

  <!-- everything goes inside of these divs -->
  <div class="giant-container" style="border: 1px solid red; height: 100vh;">

      <h1>Hello Welcome to CodeCalendar.com!</h1>
      <img src="../media/code_calanderV1.png" width="40%"/>
      <p>All of our stuff should go between these template tags surrounding this code</p>
      <p>Styles for everything on this page can be added below in the style tag</p>
      <p>inside of the script below is where we can add variables and lifecycle hooks</p>
  <div class="calendar">
      <div class="calendar-header">
          <i class="fa fa-fw fa-chevron-left" @click="subtractMonth"></i>
          <h4>{{month + ' - ' + year}}</h4>
          <i class="fa fa-fw fa-chevron-right" @click="addMonth"></i>
      </div>
      <ul class="weekdays">
        <li v-for="day in days" :key="day"></li>
      </ul>
      <ul class="dates">
        <li v-for="blank in firstDayOfMonth" :key="blank">&nbsp;</li>
        <li v-for="date in daysInMonth" 
        :class="{'current-day': date == initialDate &amp;&amp; month == initialMonth && year == initialYear}" :key="date" >;
        <span></span>
        </li>
      </ul>
    </div>    
  </div> 
</template>

<script>

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
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
