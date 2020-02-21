<template>
  <div>
    <img src="@/assets/images/topic-images/topic3.png"/>
    <pre style="font-size: 20px">{{code}}</pre>
    <img src="@/assets/images/topic-images/topic3_success.png"/>
    <pre style="font-size: 20px">{{code1}}</pre>
  </div>
</template>

<script>
export default {
  name: 'topic3',
  data () {
    return {
      code: 'public char firstUniqChar(String s) {\n' +
        '        //使用LinkedHashMap可以保持顺序\n' +
        '        Map<Character, Integer> map = new LinkedHashMap<>();\n' +
        '        for (int i = 0; i < s.length(); i++) {\n' +
        '            char tmp = s.charAt(i);\n' +
        '            if (map.containsKey(tmp))\n' +
        '                map.put(tmp, map.get(tmp) + 1);\n' +
        '            else\n' +
        '                map.put(tmp, 1);\n' +
        '        }\n' +
        '        //判断是否存在只出现1次的字符\n' +
        '        if (map.containsValue(1)) {\n' +
        '            for (Map.Entry<Character, Integer> entry : map.entrySet()) {\n' +
        '                if (entry.getValue() == 1)\n' +
        '                    return entry.getKey();\n' +
        '            }\n' +
        '        }\n' +
        '        return " ".charAt(0);\n' +
        '}',
      code1: '\n最优解：\npublic char firstUniqChar(String s) {\n' +
        '        char[] chars = new char[26];\n' +
        '        char[] chars1 = s.toCharArray();\n' +
        '        for (char c : chars1) {\n' +
        '            chars[c - \'a\']++;\n' +
        '        }\n' +
        '        for (char c : chars1) {\n' +
        '            if (chars[c-\'a\']==1) return c;           \n' +
        '        }\n' +
        '        return \' \';\n' +
        '    }'
    }
  }
}
</script>

<style scoped>

</style>
