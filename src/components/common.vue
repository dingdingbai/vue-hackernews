<template lang="pug">
  .container
    header
      nav
        img(src='../assets/logo.png')
        router-link(to='/top') Top
        router-link(to='/new') New
        router-link(to='/show') Show
        router-link(to='/ask') Ask
        router-link(to='/job') Jobs
        p Bulid by BY
    .main
      router-view  
</template>

<script>
  
</script>

<style lang="stylus">  
  .container
    display: flex
    flex-direction: column
    height: 100vh 
    header
      background: #f60
      nav
        max-width: 800px
        display: flex
        align-items: center
        margin: auto
        color: white
        padding: 20px 0
        > a
          text-decoration: none
          margin-right: 30px
          font-weight: 500
          color: white
        .router-link-active {
          font-weight: 700
        }
      img
        width: 24px
        margin-right: 30px
      p
        margin-left: auto
    .main
      flex: 1
      overflow: auto
      // padding: 20px 0
      .main-container
        > ul
          padding: 0
  
</style>