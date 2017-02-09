<template lang='pug'>
  div
    h1 This is Page 2
    p Go back #[nuxt-link(to='/') Home] (I used #[code nuxt-link] here).
    p This page was written using #[a(href='https://pugjs.org', target='_blank') Pug]
    p.highlight.
      This is a block
      of text that is
      a bit long
      and it will turn out highlighted.
    p A message from Vue: #[span.message {{ message }}]
</template>

<script>
export default {
  // It's OK to use an object for head instead of a function.
  head: {
    title: 'Page Two'
  },
  data() {
    return {message: 'Cool message from the data() method'}
  }
}
</script>

<style lang='stylus'>
p.highlight
  background-color: palegoldenrod
span.message
  color: steelblue
  font-weight: bold
  font-size: 1.2rem
  font-family: monospace
  text-decoration: underline
</style>
