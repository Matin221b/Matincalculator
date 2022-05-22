<script>
export default {
  props: {
 
  },
 
  methods: {
  }
}; 
</script>

<template>
  <div>
    <table id="calculator" dir="rtl" border="1">
      <tr>
      
        <td colspan="4">
          <input v-model="screen" dir="ltr" id="display" type="number"/>
        </td>
      
      </tr>
      <tr>
        <td><button @click="clear" id="clear">C</button></td>
        <td><button @click="del" id="delete">del</button></td>
        <td><button @click="point()" id="point" class="point">.</button></td>
        <td><button @click="mod" id="mod">%</button></td>
      </tr>
      <tr>
        <td><button @click="div" id="div">/</button></td>
        <td><button @click="digit(9)" id="digit" class="digit">9</button></td>
        <td><button @click="digit(8)" id="digit" class="digit">8</button></td>
        <td><button @click="digit(7)" id="digit" class="digit">7</button></td>
      </tr>
      <tr>
        <td><button @click="mul" id="mul">*</button></td>
        <td><button @click="digit(6)" id="digit" class="digit">6</button></td>
        <td><button @click="digit(5)" id="digit" class="digit">5</button></td>
        <td><button @click="digit(4)" id="digit" class="digit">4</button></td>
      </tr>
      <tr>
        <td><button @click="minus" id="minus">-</button></td>
        <td><button @click="digit(3)" id="digit" class="digit">3</button></td>
        <td><button @click="digit(2)" id="digit" class="digit">2</button></td>
        <td><button @click="digit(1)" id="digit" class="digit">1</button></td>
      </tr>
      <tr>
        <td colspan="2"><button @click="equal" id="equal">=</button></td>
        <td><button @click="digit(0)" id="digit" class="digit">0</button></td>
        <td><button @click="sum" id="sum">+</button></td>
      </tr>
    </table>
  </div>
</template>

<style>
#calculator {
  text-align: center;
  margin: auto
}
#display {
padding: 5px;
font-weight: bold;
text-align: right
}
#equal {
  background-color: rgb(89, 89, 210);
  border: 1px solid rgb(89, 89, 210);
  width: calc(100%);
  padding: 10px 0;
}
#delete {
  background-color: rgb(210, 140, 89);
  border: 1px solid rgb(210, 140, 89);
  width: calc(100%);
  padding-bottom: 10px;
  padding-top: 10px;
}
#digit{
  background-color: rgb(255, 255, 255);
  border: 1px solid rgb(0, 0, 0);
  width: calc(100%);
  padding: 10px;
}
#point {
  background-color: rgb(201, 113, 255);
  border: 1px solid rgb(201, 113, 255);
  width: calc(100%);
  padding: 10px
}
#sum {
  background-color: rgb(210, 89, 200);
  border: 1px solid rgb(210, 89, 200);
  width: calc(100%);
  padding: 10px
}
#minus {
  background-color: rgb(89, 210, 89);
  border: 1px solid rgb(89, 210, 89);
  width: calc(100%);
  padding: 10px
}
#mul {
  background-color: rgb(200, 210, 89);
  border: 1px solid rgb(200, 210, 89);
  width: calc(100%);
  padding: 10px
}
#clear {
  background-color: rgb(210, 89, 89);
  border: 1px solid rgb(210, 89, 89);
  width: calc(100%);
  padding: 10px
}
#div {
  background-color: rgb(89, 210, 208);
  border: 1px solid rgb(89, 210, 208);
  width: calc(100%);
  padding: 10px
}
#mod {
  background-color: rgb(255, 209, 125);
  border: 1px solid rgb(255, 209, 125);
  width: calc(100%);
  padding: 10px
}
</style>