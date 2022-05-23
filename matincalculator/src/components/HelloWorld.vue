<script>
</script>

<template>
  <div>
    <table id="calculator" dir="rtl">  <!--جدول و دکمه‌های ماشین حساب-->
      <tr>
      
        <td colspan="4">
          <input v-model="screen" dir="ltr" id="display" type="number"/>   <!--اضافه کردن صفحه نمایش-->
        </td>
      
      </tr>
      <tr>
        <td><button @click="mul" id="mul">*</button></td>   <!--اضافه کردن دکمه‌ی ضربدر-->
        <td><button @click="mod" id="mod">%</button></td>   <!--اضافه کردن دکمه‌ی درصد-->
        <td colspan="2"><button @click="clear" id="clear">C</button></td>    <!--اضافه کردن دکمه‌ی پاک کردن صفحه نمایش-->
      </tr>
      <tr>
        <td><button @click="div" id="div">/</button></td>   <!--اضافه کردن دکمه‌ی تقسیم-->
        <td><button @click="digit(9)" id="digit" class="digit">9</button></td>   <!--9اضافه کردن دکمه‌ی عدد-->
        <td><button @click="digit(8)" id="digit" class="digit">8</button></td>   <!--8اضافه کردن دکمه‌ی عدد-->
        <td><button @click="digit(7)" id="digit" class="digit">7</button></td>   <!--7اضافه کردن دکمه‌ی عدد-->
      </tr>
      <tr>
        <td><button @click="minus" id="minus">-</button></td>    <!--اضافه کردن دکمه‌ی تفریق-->
        <td><button @click="digit(6)" id="digit" class="digit">6</button></td>   <!--6اضافه کردن دکمه‌ی عدد-->
        <td><button @click="digit(5)" id="digit" class="digit">5</button></td>   <!--5اضافه کردن دکمه‌ی عدد-->
        <td><button @click="digit(4)" id="digit" class="digit">4</button></td>   <!--4اضافه کردن دکمه‌ی عدد-->
      </tr>
      <tr>
        <td><button @click="sum" id="sum">+</button></td>    <!--اضافه کردن دکمه‌ی جمع-->
        <td><button @click="digit(3)" id="digit" class="digit">3</button></td>   <!--3اضافه کردن دکمه‌ی عدد-->
        <td><button @click="digit(2)" id="digit" class="digit">2</button></td>   <!--2اضافه کردن دکمه‌ی عدد-->
        <td><button @click="digit(1)" id="digit" class="digit">1</button></td>   <!--1اضافه کردن دکمه‌ی عدد-->
      </tr>
      <tr>
        <td colspan="2"><button @click="equal" id="equal">=</button></td>    <!--اضافه کردن دکمه‌ی مساوی-->
        <td colspan="2"><button @click="digit(0)" id="digit" class="digit">0</button></td>   <!--0اضافه کردن دکمه‌ی عدد-->
      </tr>
    </table>
  </div>
</template>
<!--تغییرات ظاهری ماشین حساب-->
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
  border: 2px solid black;
  width: calc(100%);
  padding: 11.5px 0;
}
#digit{
  font: message-box;
  color: black;
  background-color:rgb(82, 190, 128);
  border: 2px solid rgb(0, 0, 0);
  width: calc(100%);
  padding: 10px;
}
#sum {
  color: white;
  background-color: #2c3e50;
  border: 2px solid black;
  width: calc(100%);
  padding: 11.5px
}
#minus {
  color: white;
  background-color: #2c3e50;
  border: 2px solid black;
  width: calc(100%);
  padding: 11.5px
}
#mul {
  color: white;
  background-color: #2c3e50;
  border: 2px solid black;
  width: calc(100%);
  padding: 11.5px
}
#clear {
  color: white;
  background-color: #2c3e50;
  border: 2px solid black;
  width: calc(100%);
  padding: 11.5px
}
#div {
  color: white;
  background-color: #2c3e50;
  border: 2px solid black;
  width: calc(100%);
  padding: 11.5px
}
#mod {
  color: white;
  background-color: #2c3e50;
  border: 2px solid black;
  width: calc(100%);
  padding: 11.5px
}
</style>