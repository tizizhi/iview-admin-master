<template>
  <div>
    <img src="@/assets/images/topic-images/topic11.png"/><br/><br/>
    <pre style="font-size: 20px">{{code}}</pre>
    <img src="@/assets/images/topic-images/topic11_success.png"/><br/><br/><br/><br/>
  </div>
</template>

<script>
export default {
  name: 'topic8',
  data () {
    return {
      code: 'public ListNode addTwoNumbers(ListNode l1, ListNode l2) {\n' +
        '        ListNode node = new ListNode(0);\n' +
        '        //记录链表最新位置\n' +
        '        ListNode cursor = node;\n' +
        '        ListNode next;\n' +
        '        //是否满10进位\n' +
        '        int p = 0;\n' +
        '        while (true) {\n' +
        '            int sum = (l1 == null ? 0 : l1.val) + (l2 == null ? 0 : l2.val) + p;\n' +
        '            if (sum >= 10) {\n' +
        '                next = new ListNode(sum - 10);\n' +
        '                p = 1;\n' +
        '            } else {\n' +
        '                next = new ListNode(sum);\n' +
        '                p = 0;\n' +
        '            }\n' +
        '            cursor.next = next;\n' +
        '            cursor =  cursor.next;\n' +
        '            if (l1 != null)\n' +
        '                l1 = l1.next;\n' +
        '            if (l2 != null)\n' +
        '                l2 = l2.next;\n' +
        '            if (l1 == null && l2 == null && p != 1)\n' +
        '                break;\n' +
        '        }\n' +
        '        return node.next;\n' +
        '}'
    }
  }
}
</script>

<style scoped>

</style>
