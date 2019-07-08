<template>
  <div id="app">
      <div>
          Vue实例
          <li v-for="(list,index) in listData" :key="index" @click="handClick(index)">
            {{list.name}}
          </li>
      </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      listData:[{
        name:"lalal"
      },{
        name:"wowow"
      },{
        name:"dudud"
      }]
    }
  },
  methods: {
    handClick(index){
      console.log(index)
    }
  },
}
</script>

<style lang="scss">

</style>
