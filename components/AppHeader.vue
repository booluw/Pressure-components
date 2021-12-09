<template>
  <header class="header">
    <input type="checkbox" class="hamburger__toggler" id="main-toggler" />
    <div class="header__main">
      <img src="img/pci_lrge_logo.png" class="header__logo" alt="Pressure Component Logo" />
      <div class="header__desktop-only">
        <div class="header-card">
          <i class="header-card__icon fa fa-map-marker">
          </i>
          <div>
            5101 Naiman Parkway Solon,<br /> OH 44139
          </div>
        </div>
        <div class="header-card">
          <i class="header-card__icon fa fa-phone">
          </i>
          <div>
            440-325-0306
            <br />
            sales@pressurecomponent.com
          </div>
        </div>
        <nuxt-link to="contact-us" class="header__btn btn btn--cta">
          request a quote
        </nuxt-link>
      </div>
    </div>
    <nav class="header__nav">
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
      <a href="#search" @click.prevent="openModal()" class="header__search-icon fa fa-search"></a>
    </nav>
    <label class="hamburger" for="main-toggler">
      <div class="hamburger__line"></div>
      <div class="hamburger__line"></div>
      <div class="hamburger__line"></div>
    </label>
  </header>
</template>

<script>
export default {
  name: 'AppHeader'
}
</script>
