<template>
  <section class="jumbotron">
    <div class="row m-0 align-items-center justify-content-between">
      <div class="col-md-7 p-0">
        <h1 class="jumbotron__heading">
          We are a leading supplier of quality hydraulic components
        </h1>
        <div class="row m-0 justify-content-between" style="text-align: center; margin: 3rem 0 0;">
          <div class="col-md-5 p-0">
            <a href="~/static/doc/PCI-HOSE-FITTING-LIST-PRICING-2021.pdf" class="btn btn--big btn--bordered" download>New Custom Fitting Line</a>
          </div>
          <div class="col-md-5 p-0">
            <nuxt-link to="stocking-in-mexico"  class="btn btn--big btn--bordered" download>Now Stocking in Mexico</nuxt-link>
          </div>
        </div>
      </div>
      <div class="col-md-3 p-0">
        <a href="~/static/docs/2021-PCI-Catalog-update-Sept-digital-compressed.pdf" download>
          <img src="~/static/img/Click-to-View-the-2021-Catalog.png" class="jumbotron__img" />
        </a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'AppJumbotron'
}
</script>
