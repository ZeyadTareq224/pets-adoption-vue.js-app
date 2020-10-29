<template>
  <div>
    <petsTable species="dogs" :pets="dogs"/>
  </div>
</template>

<script>
import petsTable from '@/components/petsTable.vue'
import { mapState } from 'vuex'

export default {
  name: "Dog",
  components:{
    petsTable
  },
  data(){
    return{}
  },
  computed: {
    ...mapState([
      'dogs'
    ])
  }
}
</script>

<style>

</style>