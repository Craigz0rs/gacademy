<template>
  <div class="layout">
    <header class="site-header header-unscrolled">
      <div class="header-overlays">
        <div class="header-overlay1"></div>
        <div class="header-overlay2"></div>
        <div class="header-overlay3"></div>
      </div>
      <div class="site-branding">
        <g-link class="custom-logo-link" to="/">
          <g-image src=""/>
        </g-link>
      </div>
      <nav class="main-navigation">
        <g-link class="nav__link" to="/">Home</g-link>
        <g-link class="nav__link" to="/about">Our School</g-link>
        <g-link class="nav__link" to="/">Student Life</g-link>
        <g-link class="nav__link" to="/">News</g-link>
        <g-link class="nav__link" to="/contact">Contact</g-link>
      </nav>
    </header>
    <slot />
  </div>
</template>

<static-query>
query {
  metaData {
    siteName
  }
}
</static-query>

<style>
body {
  font-family: -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Roboto,
    "Helvetica Neue", Arial, sans-serif;
  margin: 0;
  padding: 0;
  line-height: 1.5;
}

.layout {
  max-width: 760px;
  margin: 0 auto;
  padding-left: 20px;
  padding-right: 20px;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
}

.nav__link {
  margin-left: 20px;
}
</style>
