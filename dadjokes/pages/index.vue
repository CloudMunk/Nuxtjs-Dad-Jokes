<template>
  <div class="container">
    <h2>
        Welcome to the best corny dad jokes app on the web
    </h2>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  head() {
      return {
          title: 'Welcome to Dad Jokes',
          meta: [
              {
                  hid: 'description',
                  name: 'description',
                  content: 'Best place fo corny dad jokes'
              }
          ]
      }
  }
}
</script>

