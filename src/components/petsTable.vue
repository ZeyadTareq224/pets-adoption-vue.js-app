<template>
  <div>
    <h1>{{ speciec }} For Adoption</h1>
    <b-table striped hover :items="pets">
      <template #cell(name)="data">
        <router-link :to="`pets/${speciec}/${data.index}`">{{ data.value }}</router-link>
      </template>
    </b-table>
  </div>
</template>

<script>
export default {
    props:{
        speciec: String,
        pets: Array
    }
}
</script>

<style>

</style>