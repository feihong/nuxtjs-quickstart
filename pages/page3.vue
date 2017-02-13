<template lang='pug'>
  div
    h1 This is Page 3
    p Go back #[nuxt-link(to='/') Home].
    p Unfortunately, not the most interesting page.
</template>

<script>
export default {
  head: {
    title: 'Page Three'
  },
  layout: 'another'
}
</script>
