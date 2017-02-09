<template>
  <div>
    <h1>Hello world!</h1>

    <p>{{ greeting }}</p>
    <p>
      <button v-on:click='updateGreeting'>Click me!</button>
    </p>
    <p>
      <nuxt-link to='/page2'>Check out Page 2</nuxt-link>
    </p>
  </div>
</template>

<script>
const greetings = [
    'Hello World',
    'Hola Mundo',
    'ਸਤਿ ਸ੍ਰੀ ਅਕਾਲ ਦੁਨਿਆ',
    'こんにちは世界',
    '你好世界',
    'Përshendetje Botë',
    'مرحبا بالعالم',
    'Բարեւ, աշխարհ',
    'হ্যালো দুনিয়া',
    'Saluton mondo',
    'გამარჯობა მსოფლიო',
]

function getGreeting() {
  let index = Math.floor(Math.random() * greetings.length)
  return greetings[index]
}

export default {
  data() {
    return {greeting: getGreeting()}
  },
  head() {
    return {title: 'Hello World!'}
  },
  methods: {
    updateGreeting() {
      this.greeting = getGreeting()
    }
  }
}
</script>
