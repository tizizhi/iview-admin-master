<template>
  <div>
    <pre style="font-size: 20px">{{code}}</pre>
  </div>
</template>

<script>
export default {
  name: 'topic1',
  data () {
    return {
      code: 'public int[] twoSum(int[] nums, int target) {\n' +
        '   int []a=new int[2];\n' +
        '   for(int i=0;i<nums.length;i++){\n' +
        '       for(int j=i+1;j<nums.length;j++){\n' +
        '           if(nums[i]+nums[j]==target){\n' +
        '               a=new int[]{i,j};\n' +
        '           }\n' +
        '       }\n' +
        '   }\n' +
        '   return a;\n' +
        '}'
    }
  }
}
</script>

<style scoped>

</style>
