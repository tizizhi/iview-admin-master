<template>
  <div>
    <Card shadow>
      <Row>
        <i-col span="4">
          <Button @click="createTagParams(1)">详解</Button>
        </i-col>
        <i-col span="20">
          <p>两数之和</p>
        </i-col>
      </Row>
    </Card>
    <Card shadow style="margin-top: 10px;">
      <Row>
        <i-col span="4">
          <Button @click="createTagParams(2)">详解</Button>
        </i-col>
        <i-col span="20">
          <p>单词距离</p>
        </i-col>
      </Row>
    </Card>
    <Card shadow style="margin-top: 10px;">
      <Row>
        <i-col span="4">
          <Button @click="createTagParams(3)">详解</Button>
        </i-col>
        <i-col span="20">
          <p>第一个只出现一次的字符</p>
        </i-col>
      </Row>
    </Card>
    <Card shadow style="margin-top: 10px;">
      <Row>
        <i-col span="4">
          <Button @click="createTagParams(4)">详解</Button>
        </i-col>
        <i-col span="20">
          <p>只有两个键的键盘</p>
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
