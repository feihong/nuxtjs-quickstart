<template lang='pug'>
  div
    h1 This is Page 2
    p This page was written using #[a(href='https://pugjs.org', target='_blank') Pug]
    p.highlight.
      This is a block
      of text that is
      a bit long
      and it will turn out highlighted.
</template>

<script>
export default {
  // It's OK to use an object for head instead of a function.
  head: {
    title: 'Page Two'
  }
}
</script>

<style>
p.highlight {
  background-color: palegoldenrod;
}
</style>
