<template>
    <div>
      <ul>
        <li v-for="(m) in messages" :key="m.id">
          <a href="">{{m.title}}</a>
        </li>
      </ul>
    </div>
</template>

<script>
export default {
  name: 'Message',
  data () {
    return {
      messages: []
    }
  },
  mounted () {
    // 模拟ajax请求
    setTimeout(() => {
      const messages = [
        {
          id: 1,
          title: 'message001'
        },
        {
          id: 2,
          title: 'message002'
        },
        {
          id: 3,
          title: 'message003'
        },
        {
          id: 4,
          title: 'message004'
        },
        {
          id: 5,
          title: 'message005'
        }
      ]
      this.messages = messages
    }, 1000)
  }
}
</script>

<style scoped>

</style>
