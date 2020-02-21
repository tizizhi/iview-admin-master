<template>
  <div>
    <img src="@/assets/images/topic-images/topic2.png"/>
    <pre style="font-size: 20px">{{code}}</pre>
    <img src="@/assets/images/topic-images/topic2_success.png"/>
  </div>
</template>

<script>
export default {
  name: 'topic2',
  data () {
    return {
      code: 'public int findClosest(String[] words, String word1, String word2) {\n' +
        '        //第一次解法\n' +
        '        //首先利用字符串建立两个数组，分别记录word1和word2在words出现的位置\n' +
        '        String a = "";\n' +
        '        String b = "";\n' +
        '        for (int i = 0; i < words.length; i++) {\n' +
        '            if (words[i].equals(word1)) {\n' +
        '                a += i + " ";\n' +
        '            }\n' +
        '            if (words[i].equals(word2)) {\n' +
        '                b += i + " ";\n' +
        '            }\n' +
        '        }\n' +
        '        String[] s1 = a.length() >= b.length() ? a.split(" ") : b.split(" ");\n' +
        '        String[] s2 = a.length() < b.length() ? a.split(" ") : b.split(" ");\n' +
        '        int min = words.length;\n' +
        '        //遍历，取出差值为最小的即最短距离\n' +
        '        for (int i = 0; i < s2.length; i++) {\n' +
        '            for (int j = 0; j < s1.length; j++) {\n' +
        '                int tmp = Integer.valueOf(s2[i]) - Integer.valueOf(s1[j]);\n' +
        '                tmp = tmp < 0 ? -tmp : tmp;\n' +
        '                min = min < tmp ? min : tmp;\n' +
        '            }\n' +
        '        }\n' +
        '        return min;\n' +
        '}'
    }
  }
}
</script>

<style scoped>

</style>
