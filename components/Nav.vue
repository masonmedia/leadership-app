<template>
    <b-navbar fixed="top" toggleable="xl" type="light" variant="light">
        <NuxtLink to="/">
        <b-img src="~assets/img/Loblaws.png" style="width: 130px"></b-img>
            <b-navbar-brand class="font-weight-bold pb-0 align-middle">Lead for Life</b-navbar-brand>
        </NuxtLink>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav class="ml-auto">
        <NuxtLink class="nav-item text-secondary" to="/home">Home</NuxtLink>
        <!-- <NuxtLink class="nav-item text-secondary" to="/">Home</NuxtLink> -->
        <!-- <b-nav-item href="#" disabled>Disabled</b-nav-item> -->
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav>
        <b-nav-item-dropdown text="Lang" right>
          <b-dropdown-item href="#">EN</b-dropdown-item>
          <b-dropdown-item href="#">ES</b-dropdown-item>
          <b-dropdown-item href="#">RU</b-dropdown-item>
          <b-dropdown-item href="#">FA</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>
export default {
    name: 'Nav',
}
</script>