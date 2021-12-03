<template>
  <section>
    <app-header />
    <nuxt-child />
    <footer class="footer">
      Footer Goes Here
    </footer>
  </section>
</template>

<script>
export default {
   name: 'DefaultView'
}
</script>