<template>
  <div>
    <img src="@/assets/images/topic-images/topic10.png"/><br/><br/>
    <pre style="font-size: 20px">{{code}}</pre>
  </div>
</template>

<script>
export default {
  name: 'topic8',
  data () {
    return {
      code: 'public int add(int a, int b) {\n' +
          '        return Math.addExact(a, b);\n' +
          '}'
    }
  }
}
</script>

<style scoped>

</style>
