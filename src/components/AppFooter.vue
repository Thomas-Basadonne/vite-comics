<script>
export default {
  data() {
    return {
      dcComicsLinks: [
        {
          label: "Characters",
          link: "#",
        },
        {
          label: "Comics",
          link: "#",
        },
        {
          label: "Movies",
          link: "#",
        },
        {
          label: "TV",
          link: "#",
        },
        {
          label: "Games",
          link: "#",
        },
        {
          label: "Videos",
          link: "#",
        },
        {
          label: "News",
          link: "#",
        },
      ],
      shopLinks: [
        {
          label: "Shop DC",
          link: "#",
        },
        {
          label: "Shop DC Collectibles",
          link: "#",
        },
      ],
      dcLinks: [
        {
          label: "Term Of Use",
          link: "#",
        },
        {
          label: "Privacy Policy(New)",
          link: "#",
        },
        {
          label: "Ad Choices",
          link: "#",
        },
        {
          label: "Advertising",
          link: "#",
        },
        {
          label: "Jobs",
          link: "#",
        },
        {
          label: "Subscriptions",
          link: "#",
        },
        {
          label: "Talent Workshops",
          link: "#",
        },
        {
          label: "CPSC Certificates",
          link: "#",
        },
        {
          label: "Ratings",
          link: "#",
        },
        {
          label: "Shop Hepl",
          link: "#",
        },
        {
          label: "Contact Us",
          link: "#",
        },
      ],
      sitesLinks: [
        {
          label: "DC",
          link: "#",
        },
        {
          label: "MAD Magazine",
          link: "#",
        },
        {
          label: "DC Kids",
          link: "#",
        },
        {
          label: "TV",
          link: "#",
        },
        {
          label: "DC Universe",
          link: "#",
        },
        {
          label: "DC Power Visa",
          link: "#",
        },
      ],
    };
  },
};
</script>
<template>
  <section>
    <footer>
      <div class="container d-flex">
        <div class="col d-flex">
          <div class="comics-link">
            <h3>DC COMICS</h3>
            <ul>
              <li v-for="link in dcComicsLinks" :key="link.label">
                {{ link.label }}
              </li>
            </ul>

            <h3>SHOP</h3>
            <ul>
              <li v-for="link in shopLinks" :key="link.label">
                {{ link.label }}
              </li>
            </ul>
          </div>

          <div class="dc-links">
            <h3>DC</h3>
            <ul>
              <li v-for="link in dcLinks" :key="link.label">
                {{ link.label }}
              </li>
            </ul>
          </div>

          <div class="sites-links">
            <h3>SITES</h3>
            <ul>
              <li v-for="link in sitesLinks" :key="link.label">
                {{ link.label }}
              </li>
            </ul>
          </div>
        </div>
        <div class="img-logo">
          <img src="../assets/img/dc-logo-bg.png" alt="" />
        </div>
      </div>
    </footer>
  </section>

  <section class="social">
    <div class="container d-flex">
      <span class="btn">SING-UP NOW</span>
      <div class="links d-flex">
        <span>FOLLOW US</span>
        <ul class="d-flex">
          <li><img src="../assets/img/footer-facebook.png" alt="" /></li>
          <li><img src="../assets/img/footer-twitter.png" alt="" /></li>
          <li><img src="../assets/img/footer-youtube.png" alt="" /></li>
          <li><img src="../assets/img/footer-pinterest.png" alt="" /></li>
          <li><img src="../assets/img/footer-periscope.png" alt="" /></li>
        </ul>
      </div>
    </div>
  </section>
</template>
<style lang="scss" scoped>
footer {
  background-image: url(../assets/img/footer-bg.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  color: white;
}
.col {
  width: 50%;
  gap: 40px;
  padding: 3rem 0;
  h3 {
    margin: 1rem 0;
  }
  li {
    margin: 7px 0;
    color: hsl(0deg 0% 47%);
    &:hover {
      color: white;
    }
  }
}
img {
  width: 85%;
}

.social {
  background-color: #303030;
}
.container {
  justify-content: space-between;
  align-items: center;
}
.btn {
  margin: 3rem 0;
  padding: 10px;
  border: 1px solid #0282f9;
  color: white;
  cursor: pointer;
  &:hover {
    background-color: white;
    color: #0282f9;
  }
}
.links span {
  font-size: larger;
  line-height: 50px;
  color: #0282f9;
  font-weight: bold;
}
li {
  margin: 10px;
}
</style>
