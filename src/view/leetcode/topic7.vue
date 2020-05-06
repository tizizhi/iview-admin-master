<template>
  <div>
    <img src="@/assets/images/topic-images/topic7.png"/><br/><br/>
    <pre style="font-size: 20px">{{code}}</pre>
    <img src="@/assets/images/topic-images/topic7_success.png"/><br/><br/><br/><br/>
  </div>
</template>

<script>
export default {
  name: 'topic7',
  data () {
    return {
      code: '//Arrays.binarySearch(int[],target) 返回下标，一开始用list.contain()超时\n\n' +
        'public int lenLongestFibSubseq(int[] A) {\n' +
        '        int max = 0;\n' +
        '        for (int i = 0; i < A.length - 2; i++) {\n' +
        '            List<Integer> list = new ArrayList<>();\n' +
        '            for (int j = i + 1; j < A.length; j++) {\n' +
        '                int sum = A[i] + A[j];\n' +
        '                if (Arrays.binarySearch(A, sum) >= 0) {\n' +
        '                    int tmp = 3;\n' +
        '                    int sum1 = sum;\n' +
        '                    for (int k = j; Arrays.binarySearch(A, sum) >= 0; k = Arrays.binarySearch(A, sum1), sum1 = sum) {\n' +
        '                        sum += A[k];\n' +
        '                        if (k > j)\n' +
        '                            tmp++;\n' +
        '                    }\n' +
        '                    max = max > tmp ? max : tmp;\n' +
        '                }\n' +
        '            }\n' +
        '        }\n' +
        '        return max;\n' +
        '}'
    }
  }
}
</script>

<style scoped>

</style>
