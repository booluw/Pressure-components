<template>
  <header class="header">
    <input type="checkbox" class="hamburger__toggler" id="main-toggler" />
    <div class="header__main">
      <img src="~/static/img/pci_lrge_logo.png" class="header__logo" alt="Pressure Component Logo" />
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
            440-349-4020
            <br />
            sales@pressurecomponents.com
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
        <li class="dropdown">
          <a href="#" class="dropdown__toggler nav__link">
            products
            <span class="dropdown__arrow"></span>
          </a>
          <div class="dropdown__menu">
            <a href="~/static/docs/" class="dropdown__link" download>Quick Coupling</a>
            <a href="~/static/docs/" class="dropdown__link" download>Diagnotic and Guages</a>
            <a href="~/static/docs/" class="dropdown__link" download>High Pressure Ball Valves</a>
            <a href="~/static/docs/" class="dropdown__link" download>Pressure Wash Valves</a>
            <a href="~/static/docs/" class="dropdown__link" download>Low Pressure Ball Valves</a>
            <a href="~/static/docs/" class="dropdown__link" download>Flow Control and Needle Valves</a>
            <a href="~/static/docs/" class="dropdown__link" download>Check Valves</a>
            <a href="~/static/docs/" class="dropdown__link" download>Pipe Tube and Hose Clamps</a>
          </div>
        </li>
        <li class="dropdown">
          <a href="#" class="dropdown__toggler nav__link">
            new products
            <span class="dropdown__arrow"></span>
          </a>
          <div class="dropdown__menu">
            <a href="~/static/docs/" class="dropdown__link" download>Hydraulic Press Test Kits</a>
            <a href="~/static/docs/" class="dropdown__link" download>Pressure Wash Kits</a>
            <a href="~/static/docs/" class="dropdown__link" download>FF90 Series</a>
            <a href="~/static/docs/" class="dropdown__link" download>HSP-1040 Series</a>
            <a href="~/static/docs/" class="dropdown__link" download>HSP 1720 Series</a>
            <a href="~/static/docs/" class="dropdown__link" download>PC-100 Series Mini Needle Valves</a>
            <a href="~/static/docs/" class="dropdown__link" download>PC-400 Series Needle Valves</a>
            <a href="~/static/docs/" class="dropdown__link" download>Custom Hose Fittings</a>
          </div>
        </li>
        <li>
          <a href="~/static/docs/" class="nav__link" download>cross reference catalog</a>
        </li>
        <li>
          <nuxt-link to="/industries" class="nav__link" exact-active-class="nav__link--active">industries</nuxt-link>
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
