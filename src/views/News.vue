<template>
    <div>
      <ul>
        <li v-for="(n,index) in newsData" :key="index">{{n}}</li>
      </ul>
    </div>
</template>

<script>
export default {
  name: 'News',
  data () {
    return {
      newsData: [
        'news1',
        'news2',
        'news3',
        'news4',
        'news5'
      ]
    }
  }
}
</script>

<style scoped>

</style>
