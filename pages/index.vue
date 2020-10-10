<template>
  <section class="full-container">
    <div class="left">
      <transition name="fade">
        <div class="masked" v-if="!imgLoaded"></div>
      </transition>
    </div>
    <div class="right">
      <div class="content">
        <div class="logo">
          <object data="/logo.svg" type="image/svg+xml"></object>
        </div>
        <h1 class="title">I'm Henry Okafor</h1>
        <h5 class="sub-title">PRODUCT DESIGNER, Lagos Nigeria</h5>
        <p class="excerpt">{{bio}}</p>
        <div class="actions">
          <v-popover style="display: inline-block" offset="-100">
            <button
              target="_blank"
              href="https://drive.google.com/open?id=0BzCcry0qUvrhUGVxdDdaSHN1TnM"
              class="btn cta"
            >View Portfolio</button>
            <ul slot="popover" class="portfolios" v-close-popover>
              <li class="portfolio" v-for="portfolio in portfolios" :key="portfolio.name">
                <a :href="portfolio.link" target="_blank">
                  <svg
                    width="72px"
                    class="pdf-icon"
                    height="72px"
                    viewBox="0 0 72 72"
                    version="1.1"
                    xmlns="http://www.w3.org/2000/svg"
                    xmlns:xlink="http://www.w3.org/1999/xlink"
                  >
                    <g id="Welcome" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                      <g
                        id="My-Resume-Copy"
                        transform="translate(-1161.000000, -745.000000)"
                        fill-rule="nonzero"
                      >
                        <g id="Group-2" transform="translate(1117.000000, 702.000000)">
                          <g id="pdf-(1)" transform="translate(44.000000, 43.000000)">
                            <circle id="Oval" fill="#F0F0F0" cx="36" cy="36" r="36" />
                            <path
                              d="M21.4439517,14 C20.0946628,14 19,15.0946514 19,16.4445379 L19,55.5560738 C19,56.9059603 20.0946628,58 21.4439517,58 L49.5560483,58 C50.9059489,58 52,56.9059603 52,55.5560738 L52,25.3201144 L40.2173115,14 L21.4439517,14 Z"
                              id="Path"
                              style="fill: var(--color);"
                            />
                            <path
                              d="M52,25 L42.4890262,25 C41.114229,25 40,23.9363036 40,22.6245897 L40,14 L52,25 Z"
                              id="Path"
                              fill="rgba(0,0,0,0.3)"
                            />
                            <path
                              d="M40,41.2302099 C40,42.7600734 38.7482992,44 37.2045146,44 L16.7954854,44 C15.2510945,44 14,42.7600734 14,41.2302099 L14,32.7691895 C14,31.239326 15.2510945,30 16.7954854,30 L37.2045146,30 C38.7482992,30 40,31.239326 40,32.7691895 L40,41.2302099 Z"
                              id="Path"
                              fill="rgba(0,0,0,0.3)"
                            />
                            <g
                              id="Group"
                              transform="translate(20.000000, 34.000000)"
                              fill="#FFFFFF"
                            >
                              <path
                                d="M2.26143564,3.64076923 L1.22836634,3.64076923 L1.22836634,5.27384615 C1.22836634,5.50753846 1.1750495,5.68430769 1.06886139,5.80523077 C0.962673267,5.92615385 0.828267327,5.986 0.665940594,5.986 C0.495891089,5.986 0.359257426,5.92615385 0.255891089,5.80692308 C0.152524752,5.68769231 0.100247525,5.51215385 0.100247525,5.28138462 L0.100247525,0.835076923 C0.100247525,0.577692308 0.157425743,0.394153846 0.271336634,0.284153846 C0.385247525,0.174153846 0.566435644,0.118923077 0.814752475,0.118923077 L2.26188119,0.118923077 C2.69034653,0.118923077 3.01871287,0.152923077 3.24935644,0.221384615 C3.47717822,0.287076923 3.67440594,0.395846154 3.84,0.547846154 C4.00559406,0.699846154 4.13123762,0.886307692 4.21782178,1.10676923 C4.30440594,1.32723077 4.34673267,1.57476923 4.34673267,1.85046154 C4.34673267,2.43815385 4.17222772,2.88323077 3.82277228,3.18661538 C3.47331683,3.49 2.95277228,3.64076923 2.26143564,3.64076923 Z M1.9880198,0.996307692 L1.22836634,0.996307692 L1.22836634,2.75953846 L1.9880198,2.75953846 C2.25415842,2.75953846 2.47589109,2.73076923 2.65485149,2.67323077 C2.83262376,2.61569231 2.96881188,2.52123077 3.06267327,2.39 C3.15653465,2.25876923 3.20331683,2.08723077 3.20331683,1.87415385 C3.20331683,1.61969231 3.13113861,1.41246154 2.98663366,1.25246154 C2.82490099,1.08138462 2.49207921,0.996307692 1.9880198,0.996307692 Z"
                                id="Shape"
                              />
                              <path
                                d="M5.9879703,0.118923077 L7.45841584,0.118923077 C7.84069307,0.118923077 8.16861386,0.155692308 8.44262376,0.228923077 C8.71663366,0.302 8.96391089,0.440153846 9.18727723,0.642307692 C9.76737624,1.15630769 10.0569802,1.93815385 10.0569802,2.98753846 C10.0569802,3.33415385 10.0275743,3.65015385 9.96980198,3.93569231 C9.9120297,4.22123077 9.82143564,4.47907692 9.70024752,4.70876923 C9.57905941,4.93846154 9.4229703,5.14338462 9.23287129,5.32476923 C9.08331683,5.464 8.9199505,5.57523077 8.74277228,5.65923077 C8.56544554,5.74323077 8.37490099,5.80261538 8.17143564,5.83646154 C7.96752475,5.87046154 7.73747525,5.88769231 7.48173267,5.88769231 L6.01128713,5.88769231 C5.80618812,5.88769231 5.65173267,5.85538462 5.54777228,5.79153846 C5.44381188,5.72769231 5.37608911,5.63661538 5.34490099,5.51984615 C5.31267327,5.40292308 5.29707921,5.25153846 5.29707921,5.06507692 L5.29707921,0.835230769 C5.29707921,0.583076923 5.35158416,0.401230769 5.46044554,0.288307692 C5.56930693,0.175384615 5.74514851,0.118923077 5.9879703,0.118923077 Z M6.42475248,1.04338462 L6.42475248,4.95892308 L7.27945545,4.95892308 C7.46673267,4.95892308 7.61405941,4.95369231 7.72009901,4.94338462 C7.82628713,4.93307692 7.93678218,4.90661538 8.05069307,4.86446154 C8.16460396,4.82246154 8.26351485,4.76369231 8.34683168,4.68723077 C8.72420792,4.35676923 8.91311881,3.78753846 8.91311881,2.97923077 C8.91311881,2.40984615 8.83024752,1.984 8.66465347,1.70015385 C8.49846535,1.41692308 8.2939604,1.23615385 8.05113861,1.15907692 C7.80831683,1.082 7.51425743,1.04276923 7.16985149,1.04276923 L6.42460396,1.04276923 L6.42460396,1.04338462 L6.42475248,1.04338462 Z"
                                id="Shape"
                              />
                              <path
                                d="M14.3757921,1.01984615 L12.1535644,1.01984615 L12.1535644,2.49523077 L14.0113366,2.49523077 C14.1836139,2.49523077 14.3119307,2.53492308 14.3964356,2.61492308 C14.4813861,2.69492308 14.5237129,2.802 14.5237129,2.93553846 C14.5237129,3.06907692 14.4809406,3.17553846 14.394802,3.25446154 C14.3086634,3.33338462 14.1807921,3.37246154 14.0113366,3.37246154 L12.1535644,3.37246154 L12.1535644,5.27323077 C12.1535644,5.51446154 12.1008416,5.69338462 11.9956931,5.81030769 C11.8912871,5.92723077 11.7556931,5.98523077 11.5911386,5.98523077 C11.4239109,5.98523077 11.2877228,5.926 11.1827228,5.808 C11.0783168,5.69 11.0254455,5.51153846 11.0254455,5.27261538 L11.0254455,0.834923077 C11.0254455,0.666769231 11.0493564,0.529846154 11.0976238,0.423846154 C11.1460396,0.318 11.2210396,0.240153846 11.3238119,0.191846154 C11.4259901,0.143538462 11.5572772,0.119384615 11.7166337,0.119384615 L14.3756436,0.119384615 C14.555198,0.119384615 14.6890099,0.160769231 14.7763366,0.243076923 C14.8641089,0.326 14.9074752,0.434153846 14.9074752,0.567692308 C14.9074752,0.704153846 14.8641089,0.813538462 14.7763366,0.896461538 C14.6893069,0.978461538 14.5553465,1.01984615 14.3757921,1.01984615 Z"
                                id="Path"
                              />
                            </g>
                          </g>
                        </g>
                      </g>
                    </g>
                  </svg>
                  <span>{{portfolio.name}}</span>
                  <svg
                    class="link-icon"
                    viewBox="0 0 33 33"
                    version="1.1"
                    xmlns="http://www.w3.org/2000/svg"
                    xmlns:xlink="http://www.w3.org/1999/xlink"
                  >
                    <g id="Welcome" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                      <g
                        id="My-Resume-Copy"
                        transform="translate(-1724.000000, -897.000000)"
                        style="fill: var(--color)"
                        fill-rule="nonzero"
                      >
                        <g id="Group-2" transform="translate(1117.000000, 702.000000)">
                          <g id="link-copy" transform="translate(607.000000, 195.000000)">
                            <path
                              d="M30.9893416,1.94437245 C28.3069897,-0.647622385 23.9427054,-0.648625867 21.2624345,1.94437245 L15.2401488,7.774103 C14.8302005,8.17098026 14.8302005,8.81471417 15.2401488,9.21159143 C15.6511375,9.60897043 16.3154826,9.60897043 16.7259511,9.21159143 L22.7482369,3.38236262 C24.6096517,1.58161359 27.639003,1.58261707 29.503019,3.38236262 C31.3644339,5.18411513 31.3644339,8.11629047 29.503019,9.9170395 L21.5475254,17.6132472 C20.6464716,18.485775 19.4468007,18.9664431 18.1711749,18.9664431 C16.8960693,18.9664431 15.6958781,18.4852733 14.7937838,17.6132472 C14.3833153,17.2158682 13.7184499,17.2158682 13.3074612,17.6132472 C12.8975129,18.0101244 12.8975129,18.6538583 13.3074612,19.0507356 C14.6075383,20.3075972 16.3342112,21 18.1716951,21 C20.009179,21 21.7342912,20.3070955 23.0343683,19.0507356 L30.9898618,11.3550297 C33.6701328,8.76102786 33.6701328,4.53937774 30.9893416,1.94437245 L30.9893416,1.94437245 Z"
                              id="Path"
                            />
                            <path
                              d="M16.1357074,23.9201123 L10.2506308,29.6131055 C9.34955649,30.4856699 8.14933798,30.966358 6.87368312,30.966358 C5.5985485,30.966358 4.39780974,30.4856699 3.49777593,29.6131055 C1.63631871,27.8112777 1.63631871,24.8794815 3.49777593,23.0786572 L11.4518898,15.3826295 C13.315428,13.5823069 16.3453685,13.5823069 18.2063054,15.3826295 C18.6167833,15.7805269 19.2816638,15.7805269 19.6921416,15.3826295 C20.1026195,14.9857356 20.1026195,14.3429783 19.6921416,13.9455827 C17.0118097,11.3514724 12.6474261,11.3514724 9.96501314,13.9455827 L2.0114195,21.6406069 C-0.670473168,24.2347172 -0.670473168,28.4565438 2.0114195,31.0506541 C3.31048565,32.30807 5.03719793,33 6.87368312,33 C8.71068855,33 10.4389616,32.30807 11.7369872,31.0506541 L17.6210233,25.3581626 C18.0320214,24.9612687 18.0320214,24.3175079 17.6210233,23.9206141 C17.2110657,23.5232184 16.545665,23.5232184 16.1357074,23.9201123 L16.1357074,23.9201123 Z"
                              id="Path"
                            />
                          </g>
                        </g>
                      </g>
                    </g>
                  </svg>
                </a>
              </li>
              <li></li>
            </ul>
          </v-popover>
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
import { bio } from "~/package.json";
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
        content: bio.substr(0, 150)
      }
    ]
  }),
  data: () => ({
    bio,
    imgUrl: require("~/assets/img/Henry-Image.jpg"),
    imgLoaded: false,
    portfolios: [
      { name: "Web Design Portfolio", link: "https://drive.google.com/file/d/1C-i4kiPsbosdPJNpfI85TLeOFXZTzRyo/view?usp=sharing" },
      { name: "Mobile Design Portfolio", link: "https://drive.google.com/file/d/1eSvpzsWTgBt_ssKOHSOQAo2_P0DFWVu7/view?usp=sharing" }
    ]
  }),
  mounted() {
    const img = new Image();
    console.log("mounted");
    img.onload = () => {
      console.log("image loaded");
      this.imgLoaded = true;
    };
    img.src = this.imgUrl;
  }
};
</script>

<style lang="scss">
.popover {
  border-radius: 8px;
  background: white;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
  max-width: 80%;
  width: 280px;
}
.portfolios {
  list-style: none;
  padding: 0;
  .portfolio {
    --color: #666;
    a {
      color: var(--color);
      display: flex;
      padding: 12px 15px;
      align-items: center;
      text-decoration: none;
      > svg,
      > span {
        vertical-align: middle;
      }
    }
    :hover{
      --color: #ea0e68;
    }
  }
  .pdf-icon {
    --size: 30px;
    width: var(--size);
    height: var(--size);
    margin-right: 20px;
  }
  .link-icon {
    --size: 15px;
    width: var(--size);
    height: var(--size);
    margin-left: auto;
  }
}
.fade {
  &-enter-active,
  &-leave-active {
    transition: opacity 0.5s ease-in-out;
  }
  &-leave-to,
  &-enter {
    opacity: 0;
  }
}
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
    position: relative;
    background: url("~assets/img/Henry-Image.jpg");
    background-size: cover;
    background-position: center center;
  }
  .masked {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-image: linear-gradient(180deg, #b73648, #631724);
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
        background: linear-gradient(0deg, rgba(0,0,0,90%) 50%, transparent);
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
