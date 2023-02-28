<script>
export default {
  data() {
    return {
      headerLinks: [
        {
          label: "CHARACTERS",
          link: "#",
          active: false,
        },
        {
          label: "COMICS",
          link: "#",
          active: false,
        },
        {
          label: "MOVIES",
          link: "#",
          active: false,
        },
        {
          label: "TV",
          link: "#",
          active: false,
        },
        {
          label: "GAMES",
          link: "#",
          active: false,
        },
        {
          label: "COLLECTIBLES",
          link: "#",
          active: false,
        },
        {
          label: "VIDEOS",
          link: "#",
          active: false,
        },
        {
          label: "FANS",
          link: "#",
          active: false,
        },
        {
          label: "NEWS",
          link: "#",
          active: false,
        },
        {
          label: "SHOP",
          link: "#",
          active: false,
        },
      ],
    };
  },
};
</script>
<template>
  <section>
    <nav class="container">
      <img src="../assets/img/dc-logo.png" alt="logo" />
      <ul>
        <li
          v-for="link in headerLinks"
          :key="headerLinks.label"
          @mouseover="link.active = true"
          @mouseleave="link.active = false"
          :class="link.active == true ? 'active' : ''"
        >
          {{ link.label }}
        </li>
      </ul>
    </nav>
  </section>
</template>
<style lang="scss" scoped>
section {
  margin-top: 30px solid black;
}

nav {
  display: flex;
  justify-content: space-between;
  img {
    padding: 1.5rem 0;
  }
  ul {
    display: flex;
    align-items: center;
    li {
      padding: 0 0.5rem;
      height: 100%;
      line-height: 150px;
    }
  }
}

.active {
  color: #0282f9;
  box-shadow: 0 6px 3px -3px #0282f9;
}
</style>
