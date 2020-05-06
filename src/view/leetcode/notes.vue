<template>
  <div>
    <Card shadow>
      <Row>
        <i-col span="4">
          <Button @click="createTagParams(1)">详解</Button>
        </i-col>
        <i-col span="20">
          <p>1.两数之和</p>
        </i-col>
      </Row>
    </Card>
    <Card shadow style="margin-top: 10px;">
      <Row>
        <i-col span="4">
          <Button @click="createTagParams(2)">详解</Button>
        </i-col>
        <i-col span="20">
          <p>2.单词距离</p>
        </i-col>
      </Row>
    </Card>
    <Card shadow style="margin-top: 10px;">
      <Row>
        <i-col span="4">
          <Button @click="createTagParams(3)">详解</Button>
        </i-col>
        <i-col span="20">
          <p>3.第一个只出现一次的字符</p>
        </i-col>
      </Row>
    </Card>
    <Card shadow style="margin-top: 10px;">
      <Row>
        <i-col span="4">
          <Button @click="createTagParams(4)">详解</Button>
        </i-col>
        <i-col span="20">
          <p>4.只有两个键的键盘</p>
        </i-col>
      </Row>
    </Card>
    <Card shadow style="margin-top: 10px;">
      <Row>
        <i-col span="4">
          <Button @click="createTagParams(6)">详解</Button>
        </i-col>
        <i-col span="20">
          <p>6.1比特与2比特字符</p>
        </i-col>
      </Row>
    </Card>
    <Card shadow style="margin-top: 10px;">
      <Row>
        <i-col span="4">
          <Button @click="createTagParams(7)">详解</Button>
        </i-col>
        <i-col span="20">
          <p>7.最长的斐波那契子序列的长度</p>
        </i-col>
      </Row>
    </Card>
    <Card shadow style="margin-top: 10px;">
      <Row>
        <i-col span="4">
          <Button @click="createTagParams(8)">详解</Button>
        </i-col>
        <i-col span="20">
          <p>8.飞机座位分配概率</p>
        </i-col>
      </Row>
    </Card>
    <Card shadow style="margin-top: 10px;">
      <Row>
        <i-col span="4">
          <Button @click="createTagParams(10)">详解</Button>
        </i-col>
        <i-col span="20">
          <p>10.不用加号的加法</p>
        </i-col>
      </Row>
    </Card>
    <Card shadow style="margin-top: 10px;">
      <Row>
        <i-col span="4">
          <Button @click="createTagParams(11)">详解</Button>
        </i-col>
        <i-col span="20">
          <p>11.两数相加</p>
        </i-col>
      </Row>
    </Card>
  </div>
</template>

<script>
export default {
  name: 'notes',
  methods: {
    createTagParams (id) {
      const route = {
        name: 'topic' + id
      }
      this.$router.push(route)
    }

  }
}
</script>

<style scoped>

</style>
