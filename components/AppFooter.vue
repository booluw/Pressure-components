<template>
  <section>
    <div class="wrapper">
      <div class="row m-0 align-items-center justify-content-between">
        <div class="col-md-8 p-0">
          <h2 class="wrapper__heading">View Our Full <b>Catalog</b> to Learn About Our Products</h2>
        </div>
        <div class="col-md-3 p-0">
          <a href="~/static/docs/2021-PCI-Catalog-update-Sept-digital-compressed.pdf" class="wrapper__btn btn btn--cta btn--reverse" download>
            view catalog
            <i class="fa fa-arrow-right"></i>
          </a>
        </div>
      </div>
    </div>
    <footer class="footer">
      <div class="header-cards d-md-flex align-items-center">
        <div class="header-card">
          <i class="header-card__icon fa fa-map-marker">
          </i>
          <div>
            Pressure Components, Inc.<br />
            5101 Naiman Parkway<br />
            Solon, OH 44139
          </div>
        </div>
        <div class="header-card">
          <i class="header-card__icon fa fa-phone">
          </i>
          <div>
            440-325-0306
          </div>
        </div>
        <div class="header-card">
          <i class="header-card__icon fa fa-envelope-o">
          </i>
          <div>
              sales@pressurecomponent.com
          </div>
        </div>
        <div class="header-card">
          <i class="header-card__icon fa fa-clock-o">
          </i>
          <div>
              M-F: 8am - 5pm
          </div>
        </div>
      </div>
      <div class="header-cards row m-0 mt-5 py-5">
        <div class="col-md-3 mt-5 mt-md-0">
          <h2 class="footer__heading">About Us</h2>
          <p class="footer__paragraph">
            Pressure Components, Inc. was established in 1985. We are a leading supplier of quality hydraulic components including high pressure ball valves, quick disconnect couplings, diagnostic products and pipe, tube and hose clamps.
          </p>
        </div>
        <div class="col-md-3 mt-5 mt-md-0">
          <h2 class="footer__heading">Our Solutions</h2>
          <ul class="nav">
            <li>
              <nuxt-link to="/" class="nav__link" exact-active-class="nav__link--active">home</nuxt-link>
            </li>
            <li>
              <nuxt-link to="/about-us" class="nav__link" exact-active-class="nav__link--active">about us</nuxt-link>
            </li>
            <li>
              <nuxt-link to="/industries" class="nav__link" exact-active-class="nav__link--active">industries</nuxt-link>
            </li>
            <li class="dropdown">
              <a href="#" class="dropdown__toggler nav__link">
                products
                <span class="dropdown__arrow"></span>
              </a>
              <div class="dropdown__menu">
                <a href="docs/2021-PCI-Catalog-final-digital_quickcouplings.pdf" class="dropdown__link" target="_blank">Quick Coupling</a>
                <a href="docs/2021-PCI-Catalog-final-digital_diagnostics-and-gauges.pdf" class="dropdown__link" target="_blank">Diagnotic and Guages</a>
                <a href="docs/2021-PCI-Catalog-final-digital_highpressure_ballvalves-520.pdf" class="dropdown__link" target="_blank">High Pressure Ball Valves</a>
                <a href="docs/2021-PCI-Catalog-final-digital_pressure_wash_valves.pdf" class="dropdown__link" target="_blank">Pressure Wash Valves</a>
                <a href="docs/2021-PCI-Catalog-final-digital_low-medium-pressure-ball-valves.pdf" class="dropdown__link" target="_blank">Low Pressure Ball Valves</a>
                <a href="docs/2021-PCI-Catalog-final-digital_flow-control_needle-valves.pdf" class="dropdown__link" target="_blank">Flow Control and Needle Valves</a>
                <a href="docs/2021-PCI-Catalog-final-digital_check-valves.pdf" class="dropdown__link" target="_blank">Check Valves</a>
                <a href="docs/2021-PCI-Catalog-September_clamps.pdf" class="dropdown__link" target="_blank">Pipe Tube and Hose Clamps</a>
              </div>
            </li>
            <li class="dropdown">
              <a href="#" class="dropdown__toggler nav__link">
                new products
                <span class="dropdown__arrow"></span>
              </a>
              <div class="dropdown__menu">
                <nuxt-link to="new-products" class="dropdown__link">Hydraulic Press Test Kits</nuxt-link>
                <a href="docs/PW5000.pdf" class="dropdown__link" target="_blank">Pressure Wash Kits</a>
                <a href="docs/FF90.pdf" class="dropdown__link" target="_blank">FF90 Series</a>
                <a href="docs/HSP-1040-min-scaled-1.pdf" class="dropdown__link" target="_blank">HSP-1040 Series</a>
                <a href="docs/HSP1720-No-Price.pdf" class="dropdown__link" target="_blank">HSP 1720 Series</a>
                <a href="docs/PC-100-Series-Mini-Needle-Valves.pdf" class="dropdown__link" target="_blank">PC-100 Series Mini Needle Valves</a>
                <a href="docs/PC400-series-final.pdf" class="dropdown__link" target="_blank">PC-400 Series Needle Valves</a>
                <a href="docs/PCI-HOSE-FITTING-LIST-PRICING-2021.pdf" class="dropdown__link" target="_blank">Custom Hose Fittings</a>
              </div>
            </li>
            <li>
              <a href="docs/" class="nav__link" target="_blank">cross reference catalog</a>
            </li>
            <li>
              <nuxt-link to="/contact-us" class="nav__link" exact-active-class="nav__link--active">contact us</nuxt-link>
            </li>
          </ul>
        </div>
        <div class="col-md-3 mt-5 mt-md-0">
          <h2 class="footer__heading">Quick Links</h2>
          <ul class="footer__links">
            <li>
              <nuxt-link to="/about-us" class="footer__link">About Us</nuxt-link>
            </li>
            <li>
              <nuxt-link to="/contact-us" class="footer__link">Contact Us</nuxt-link>
            </li>
            <li>
              <a href="~/static/docs/2021-PCI-Catalog-update-Sept-digital-compressed.pdf" class="footer__link" download>2021 Catalog</a>
            </li>
          </ul>
        </div>
        <div class="col-md-3 mt-5 mt-md-0">
          <img src="~/static/img/pci_lrge_logo.png" />
        </div>
      </div>
      <p style="text-align: center; margin: 3rem 0 0;">
        Copyright © 2021 Pressure Components, Inc. All Rights Reserved
      </p>
    </footer>
  </section>
</template>
<script>
export default {
  name: 'AppFooter'
}
</script>