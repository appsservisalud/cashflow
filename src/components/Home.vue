<template>
  <Layout>
    <template #header>
      <Header></Header>
    </template>
    <template #resume>
      <Resume/>
    </template>
  </Layout> 
</template>

<script>
import Layout from "./Layout.vue"
import Header from "./Header.vue";
import Resume from "./Resume/index.vue"

export default{
  components:{
    Layout,
    Header,
    Resume
}
  }

</script>

<style>

@import '../assets/css/Home/home.css';

</style>

