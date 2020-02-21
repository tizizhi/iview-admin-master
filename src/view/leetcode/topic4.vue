<template>
  <div>
    <img src="@/assets/images/topic-images/topic4.png"/><br/><br/>
    <pre style="font-size: 20px">{{code}}</pre>
    <img src="@/assets/images/topic-images/topic4_success.png"/><br/><br/><br/><br/>
    <img src="@/assets/images/topic-images/topic4_answer.jpg" style="width: 95%"/>
  </div>
</template>

<script>
export default {
  name: 'topic3',
  data () {
    return {
      code: 'public int minSteps(int n) {\n' +
        '        if (n == 1)\n' +
        '            return 0;\n' +
        '        int m = 1;\n' +
        '        //获取最大因数\n' +
        '        for (int i = n / 2; i > 0; i--) {\n' +
        '            if (n % i == 0) {\n' +
        '                m = i;\n' +
        '                break;\n' +
        '            }\n' +
        '        }\n' +
        '        //递归\n' +
        '        return minSteps(m) + (n / m);\n' +
        '}\n\n\n',
      code1: ''
    }
  }
}
</script>

<style scoped>

</style>
