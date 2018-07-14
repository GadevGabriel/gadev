<template lang="pug">
  #app
    nav.nav
      .nav-container
        .logo
          a(href="/")
            img(src="./assets/logo-horizontal.png")
        ul.nav-lista
          li
            a Home
          li
            a Portfólio
          li
            a Quem sou eu?
          li
            a Contato
    router-view
</template>

<script>
export default {
  name: 'App'
}
</script>

<style lang="sass"scoped>
@import 'responsivo'

#app
  font-family: 'Avenir', Helvetica, Arial, sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  text-align: center
  color: #2c3e50

.nav
  width: 100vw
  max-width: 100%
  top: 0
  box-shadow: 0 2px 5px #ccc

.nav-container
  margin: 0 auto
  display: flex
  width: 90%
  justify-content: space-between
  align-items: center
.nav-lista
  display: flex
  justify-content: flex-end
  list-style: none

.nav-lista li
  padding: 10px 20px
  border-bottom: 3px solid white
  &:hover
    border-color: #47d278
    cursor: pointer
    color: #47d278

.logo img
  width: 120px
  height: auto
</style>
