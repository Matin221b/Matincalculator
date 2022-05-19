<script>
export default {
  props: {
 
  },
 
  methods: {
  }
}; 
</script>

<template>
  <h1>{{ msg }}</h1>

<table dir="rtl" id="btn">
<tr><input dir="rtl" type="number" id="display"></tr>
<tr>
 <td><button id="div">/</button></td>
 <td><button id="clear">C</button></td>
 <td><button id="delete">del</button></td>
</tr>
<tr>
 <td><button id="mul">*</button></td>
 <td><button id="digit">9</button></td>
 <td><button id="digit">8</button></td>
 <td><button id="digit">7</button></td>
</tr>
<tr>
 <td><button id="minus">-</button></td>
 <td><button id="digit">6</button></td>
 <td><button id="digit">5</button></td>
 <td><button id="digit">4</button></td>
</tr>
<tr>
 <td><button id="sum">+</button></td>
 <td><button id="digit">3</button></td>
 <td><button id="digit">2</button></td>
 <td><button id="digit">1</button></td>
</tr>
<tr>
 <td><button id="point">.</button></td>
 <td><button id="digit">0</button></td>
 <td><button id="equal">=</button></td>
</tr>
</table>
</template>

<style>
#equal {
  width: calc(200%);
  padding: 10px 0;
}
#delete {
  width: calc(200%);
  padding-bottom: 10px;
  padding-top: 10px;
}
#digit{
  width: calc(100%);
  padding: 10px;
}
#point {
  width: calc(100%);
  padding: 10px
}
#sum {
  width: calc(100%);
  padding: 10px
}
#minus {
  width: calc(100%);
  padding: 10px
}
#mul {
  width: calc(100%);
  padding: 10px
}
#clear {
  width: calc(100%);
  padding: 10px
}
#div {
  width: calc(100%);
  padding: 10px
}
#btn {
  margin: 0;
  padding: 0;
  border-radius: 10px;
  position: relative;
  text-align: center;
  left: 51%;
  transform: translate(-50%);
  width: calc(100% / 4 - 5px);
}
#display{
  width: calc(23%);
  position: relative;
  text-align: center;
  left: 1%;
}
</style>