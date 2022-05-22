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
    <table id="calculator" dir="rtl">
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
</style>