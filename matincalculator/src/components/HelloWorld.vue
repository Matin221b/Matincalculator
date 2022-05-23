<script>
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
        <td><button @click="mul" id="mul">*</button></td>
        <td><button @click="mod" id="mod">%</button></td>
        <td colspan="2"><button @click="clear" id="clear">C</button></td>
      </tr>
      <tr>
        <td><button @click="div" id="div">/</button></td>
        <td><button @click="digit(9)" id="digit" class="digit">9</button></td>
        <td><button @click="digit(8)" id="digit" class="digit">8</button></td>
        <td><button @click="digit(7)" id="digit" class="digit">7</button></td>
      </tr>
      <tr>
        <td><button @click="minus" id="minus">-</button></td>
        <td><button @click="digit(6)" id="digit" class="digit">6</button></td>
        <td><button @click="digit(5)" id="digit" class="digit">5</button></td>
        <td><button @click="digit(4)" id="digit" class="digit">4</button></td>
      </tr>
      <tr>
        <td><button @click="sum" id="sum">+</button></td>
        <td><button @click="digit(3)" id="digit" class="digit">3</button></td>
        <td><button @click="digit(2)" id="digit" class="digit">2</button></td>
        <td><button @click="digit(1)" id="digit" class="digit">1</button></td>
      </tr>
      <tr>
        <td colspan="2"><button @click="equal" id="equal">=</button></td>
        <td colspan="2"><button @click="digit(0)" id="digit" class="digit">0</button></td>
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
  color: white;
  background-color: #2c3e50;
  border: 1px solid #2c3e50;
  width: calc(100%);
  padding: 10px 0;
}
#digit{
  color: white;
  background-color:rgb(82, 190, 128);
  border: 1px solid rgb(0, 0, 0);
  width: calc(100%);
  padding: 10px;
}
#sum {
  color: white;
  background-color: #2c3e50;
  border: 1px solid #2c3e50;
  width: calc(100%);
  padding: 10px
}
#minus {
  color: white;
  background-color: #2c3e50;
  border: 1px solid #2c3e50;
  width: calc(100%);
  padding: 10px
}
#mul {
  color: white;
  background-color: #2c3e50;
  border: 1px solid #2c3e50;
  width: calc(100%);
  padding: 10px
}
#clear {
  color: white;
  background-color: #2c3e50;
  border: 1px solid #2c3e50;
  width: calc(100%);
  padding: 10px
}
#div {
  color: white;
  background-color: #2c3e50;
  border: 1px solid #2c3e50;
  width: calc(100%);
  padding: 10px
}
#mod {
  color: white;
  background-color: #2c3e50;
  border: 1px solid #2c3e50;
  width: calc(100%);
  padding: 10px
}
</style>