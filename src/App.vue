<template>
  <div>
    <Navbar />
    <Header />
    <HeaderLine />
    <StudentsViewing />
    <Recommendations />
    <Categories />
  </div>
</template>

<script>
import Header from './components/Header'
import HeaderLine from './components/HeaderLine'
import StudentsViewing from './components/StudentsViewing'
import Recommendations from './components/Recommendations'
import Navbar from './components/Navbar'
import Categories from './components/Categories'

export default {
  name: 'App',
  components: {
    Header,
    HeaderLine,
    StudentsViewing,
    Recommendations,
    Categories,
    Navbar
  },
  data () {
    return {
      //
    }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Open+Sans:400,600,700');

body {
  font-family: 'Open Sans', sans-serif;
}
</style>
