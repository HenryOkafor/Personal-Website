<template>
  <section class="full-container">
    <div class="left"></div>
    <div class="right">
      <div class="content">
        <div class="logo">
          <object data="/logo.svg" type="image/svg+xml"></object>
        </div>
        <h1 class="title">I'm Henry Okafor</h1>
        <h5 class="sub-title">PRODUCT DESIGNER, Lagos Nigeria</h5>
        <p class="excerpt">
          {{bio}}
        </p>
        <div class="actions">
          <a
            target="_blank"
            href="https://drive.google.com/open?id=0BzCcry0qUvrhUGVxdDdaSHN1TnM"
            class="btn cta"
          >View Portfolio</a>
          <a target="_blank" class="btn behance social" href="https://www.behance.net/HernryArts">
            <i class="fab fa-behance-square"></i>
          </a>
          <a
            target="_blank"
            class="btn linkedin social"
            href="https://www.linkedin.com/in/henry-okafor-0a82506a/"
          >
            <i class="fab fa-linkedin"></i>
          </a>
          <a target="_blank" class="btn dribbble social" href="https://dribbble.com/henryokafor">
            <i class="fab fa-dribbble-square"></i>
          </a>
        </div>
      </div>
    </div>
    <div class="toc">
      <!-- <nuxt-link to="terms-and-conditions">Terms and Conditions</nuxt-link> -->
    </div>
  </section>
</template>

<script>
import Logo from "~/components/Logo.vue";
import {bio} from "~/package.json"
// const pkg = {}
export default {
  components: {
    Logo
  },
  head: () => ({
    title: "Henry Okafor - UIUX/Product designer",
    meta: [
      {
        name: "description",
        hid: "description",
        content: bio.substr(0,150)
      }
    ]
  }),
  data:() => ({bio})
};
</script>

<style lang="scss">
.full-container {
  min-height: 100vh;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: stretch;
  text-align: center;
  .left,
  .right {
    flex: 1 0 50%;
  }

  .toc {
    position: absolute;
    bottom: 20px;
    right: 20px;
    a {
      color: black;
    }
  }
  .left {
    background: url("~assets/img/Henry-Image.jpg");
    background-size: cover;
    background-position: center center;
  }
  .right {
    align-items: center;
    display: flex;
    justify-content: center;
    text-align: left;
    .content {
      width: 100%;
      padding: 0 100px;
      .title {
        text-transform: uppercase;
        font-size: 3em;
        margin-bottom: 10px;
        font-weight: 400;
      }
      .sub-title {
        color: #ea0e68;
        font-size: 1.3em;
      }
      .logo {
        margin-bottom: 20px;
        object {
          width: 150px;
        }
      }
      .excerpt {
        margin: 20px 0;
        line-height: 1.5;
      }
      .actions {
        .cta {
          cursor: pointer;
          background: #ea0e68;
          color: white;
          font-size: 1.3em;
          height: 2.5em;
          display: inline-flex;
          text-decoration: none;
          justify-content: center;
          align-items: center;
          width: 13em;
          box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
          transition: box-shadow 0.2s ease-in-out;
          &:hover {
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
          }
          &:focus {
            background: darken($color: #ea0e68, $amount: 10%);
            outline: none;
          }
        }
        * {
          vertical-align: bottom;
        }
        .social {
          font-size: 2em;
          margin: 0 10px;
          border-collapse: collapse;
          color: #555;
          display: inline-block;
          transition: color 0.2s ease-in-out;
        }
        .dribbble:hover i {
          color: #fa398a;
        }
        .linkedin:hover {
          color: #0077ba;
        }
        .behance:hover {
          color: #0057ff;
        }
      }
    }
  }
}
@media screen and (max-width: 768px) {
  .full-container {
    position: relative;
    display: block;
    .left {
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      position: absolute;
    }
    .right {
      position: absolute;
      bottom: 0;
      left: 0;
      .content {
        padding: 0 20px 100px;
        color: white;
        .title {
          font-size: 2em;
          color: white;
        }
        .sub-title {
          font-size: 0.9em;
          color: white;
        }
        .logo {
          margin-bottom: 20px;
          object {
            width: 80px;
          }
        }
        .excerpt {
          margin: 20px 0;
          line-height: 1.5;
          font-size: 0.9em;
          font-weight: 300;
        }
        .actions {
          font-size: 0.6em;
          .cta {
            border-radius: 3px;
            background: #ea0e68;
            color: white;
            font-size: 1.3em;
            height: 2.8em;
            width: 13em;
          }
          * {
            vertical-align: bottom;
          }
          .social {
            font-size: 3em;
            margin: 0 0.3em;
            border-collapse: collapse;
            color: #fff;
            display: inline-block;
          }
        }
      }
    }
    .toc a {
      color: white;
    }
  }
}
</style>
