<template>
  <section class="full-container">
    <div class="left"></div>
    <div class="right">
      <div class="content">
        <div class="logo">
          <object data="/logo.svg" type="image/svg+xml"></object>
        </div>
        <h1 class="title">I'm Henry Okafor</h1>
        <h5 class="sub-title">UI/UX PRODUCT DESIGNER, Lagos Nigeria</h5>
        <p class="excerpt">
          I’m a visually driven creative with a keen eye for details in graphics design,
          UI design and digital product design, with more than three(3) active years
          of working experience as a UIUX team member for one of the leading
          Fintech company in Nigeria. I’m readily available to build cutting edge
          human centered digital products with you.
        </p>
        <div class="actions">
          <button class="btn cta">View Portfolio</button>
          <a class="btn social" href>
            <i class="fab fa-behance-square"></i>
          </a>
          <a class="btn social" href>
            <i class="fab fa-linkedin"></i>
          </a>
          <a class="btn social" href>
            <i class="fab fa-dribbble-square"></i>
          </a>
        </div>
      </div>
    </div>
    <div class="toc">
      <a href>Terms and Conditions</a>
    </div>
  </section>
</template>

<script>
import Logo from "~/components/Logo.vue";

export default {
  components: {
    Logo
  }
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
          background: #ea0e68;
          color: white;
          font-size: 1.3em;
          height: 2.5em;
          width: 13em;
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
          font-size: 0.7em;
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
    color: white ;
  }
  }
}
</style>
