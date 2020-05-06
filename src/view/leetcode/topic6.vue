<template>
  <div>
    <img src="@/assets/images/topic-images/topic6.png"/><br/><br/>
    <pre style="font-size: 20px">{{code}}</pre>
    <img src="@/assets/images/topic-images/topic6_success.png"/><br/><br/><br/><br/>
  </div>
</template>

<script>
export default {
  name: 'topic3',
  data () {
    return {
      code: 'public boolean isOneBitCharacter(int[] bits) {\n' +
        '        //0、11、10\n' +
        '        for (int i = 0; i < bits.length; i++) {\n' +
        '            if (i == bits.length - 1)\n' +
        '                return true;\n' +
        '            if (bits[i] == 0)\n' +
        '                continue;\n' +
        '            if (bits[i] + bits[i + 1] != 0) {\n' +
        '                i++;\n' +
        '            }\n' +
        '        }\n' +
        '        return false;\n' +
        '}',
      code1: ''
    }
  }
}
</script>

<style scoped>

</style>
