<template>
  <div>
    <petsTable speciec="cats" :pets="cats"/>
  </div>
</template>

<script>
import { mapState } from 'vuex'
import petsTable from '@/components/petsTable.vue'

export default {
  name: "Cat",
  components:{
    petsTable
  },
  data(){
    return{}
  },
  computed: {
    ...mapState([
      'cats'
    ])
  }
}
</script>

<style>

</style>