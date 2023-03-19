<template>
    <div class="navmenu">
  <b-navbar
  toggleable="lg"
  type="dark"
  variant="info"
  class="col px-md-5"
  >
    <b-navbar-brand>
      <router-link to="/" class="text-decoration-none">Home</router-link>
    </b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item>
          <router-link
          to="/login"
          class="text-decoration-none"
          >Login
        </router-link>
        </b-nav-item>
        <b-nav-item href="#" disabled>Disabled</b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-item-dropdown text="Equipe" right>
          <b-dropdown-item href="#">Alfa</b-dropdown-item>
          <b-dropdown-item href="#">Beta</b-dropdown-item>
          <b-dropdown-item href="#">Charlie</b-dropdown-item>
          <b-dropdown-item href="#">Delta</b-dropdown-item>
        </b-nav-item-dropdown>

        <b-nav-item-dropdown right>
          <!-- Using 'button-content' slot -->
          <template #button-content>
            <em>User</em>
          </template>
          <b-dropdown-item href="#">Perfil</b-dropdown-item>
          <b-dropdown-item href="#">Sair</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-collapse>
      <router-link to="/about" class="text-decoration-none">Sobre</router-link>
  </b-navbar>
</div>
</template>
<script>
</script>

<style>
  .navmenu {
    color: black;
  }
</style>
