<template>
  <div>
    <img src="@/assets/images/topic-images/topic8.png"/><br/><br/>
    <pre style="font-size: 20px">{{code}}</pre>
    <img src="@/assets/images/topic-images/topic8_success.png"/><br/><br/><br/><br/>
  </div>
</template>

<script>
export default {
  name: 'topic8',
  data () {
    return {
      code: '//根据规则，1...i...n个乘客，i座位必然有人，问题简化为n乘客是否坐到自己的位置，即50%\n' +
        'public double nthPersonGetsNthSeat(int n) {\n' +
        '        if (n == 1)\n' +
        '            return 1.0;\n' +
        '        return 0.5;\n' +
        '}'
    }
  }
}
</script>

<style scoped>

</style>
