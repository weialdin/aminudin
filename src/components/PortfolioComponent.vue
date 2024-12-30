<template>
  <div class="dizme_tm_section" id="portfolio">
    <div class="dizme_tm_portfolio">
      <div class="container">
        <div class="dizme_tm_main_title" data-align="center">
          <span>Portfolio</span>
          <h3>My Amazing Works</h3>
          <p>
            I have successfully developed a variety of projects, including an
            e-commerce website, a point of sale system, a forum platform, and a
            booking website. I am committed to continuously improving my skills
            and expanding my portfolio to align with the evolving needs of the
            company.
          </p>
        </div>
        <div class="portfolio_filter">
          <ul>
            <li>
              <a
                class="c-pointer"
                :class="activeNav === '1' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '1')"
                data-filter="*"
                >All</a
              >
            </li>
            <li>
              <a
                class="c-pointer"
                :class="activeNav === '2' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '2')"
                data-filter=".youtube"
                >Youtube</a
              >
            </li>
            <li>
              <a
                class="c-pointer"
                :class="activeNav === '3' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '3')"
                data-filter=".vimeo"
                >Point Of Sale</a
              >
            </li>
            <li>
              <a
                class="c-pointer"
                :class="activeNav === '4' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '4')"
                data-filter=".soundcloud"
                >Forum App</a
              >
            </li>
            <li>
              <a
                class="c-pointer"
                :class="activeNav === '5' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '5')"
                data-filter=".popup"
                >Booking App</a
              >
            </li>
            <li>
              <a
                class="c-pointer"
                :class="activeNav === '6' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '6')"
                data-filter=".detail"
                >Ecommerce</a
              >
            </li>
          </ul>
        </div>
        <div class="dizme_tm_portfolio_titles"></div>
        <div class="portfolio_list wow fadeInUp" data-wow-duration="1s">
          <ul class="gallery_zoom grid">
            <li class="youtube grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="Mockup Shape"
                  data-category="Youtube"
                >
                  <a
                    class="popup-youtube"
                    href="#"
                    @click.prevent="() => onClick('youtube', '7e90gBu4pas')"
                  >
                    <img src="/img/thumbs/42-56.jpg" alt="" />
                    <div
                      class="main"
                      data-img-url="/img/portfolio/weicommerce.jpeg"
                    ></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>Weialdin</h3>
                  <span>Youtube</span>
                </div>
              </div>
            </li>

            <li class="vimeo grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="Restoku"
                  data-category="Point Of Sale"
                >
                  <a
                    class="popup-vimeo"
                    href="https://github.com/weialdin/RestokuPOS"
                  >
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div
                      class="main"
                      data-img-url="/img/portfolio/restoku.jpeg"
                    ></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>Restoku</h3>
                  <span>Point Of Sale</span>
                </div>
              </div>
            </li>
            <li class="soundcloud grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="WeiOverFlow"
                  data-category="Forum App"
                >
                  <a
                    class="soundcloude_link mfp-iframe audio"
                    href="https://github.com/weialdin/WeiOverflow"
                  >
                    <img src="/img/thumbs/42-56.jpg" alt="" />
                    <div
                      class="main"
                      data-img-url="/img/portfolio/forumapp.png"
                    ></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>WeiOverFlow</h3>
                  <span>ForumApp</span>
                </div>
              </div>
            </li>
            <li class="popup grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="WeiTravel"
                  data-category="BookingApp"
                >
                  <a class="zoom" href="https://github.com/weialdin/WeiTravel">
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div
                      class="main"
                      data-img-url="/img/portfolio/weitravel.jpg"
                    ></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>WeiTravel</h3>
                  <span>Booking App</span>
                </div>
              </div>
            </li>
            <li class="detail grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="WeiCommerce"
                  data-category="Ecommerce"
                >
                  <a
                    class="portfolio_popup"
                    href="https://github.com/weialdin/WeiCommerce_FrontEnd"
                  >
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div
                      class="main"
                      data-img-url="/img/portfolio/weicommerce2.jpeg"
                    ></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>WeiCommerce</h3>
                  <span>Ecommerce</span>
                </div>
              </div>
            </li>
            <li class="detail grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="WeiCommerce Backend"
                  data-category="Ecommerce"
                >
                  <a
                    class="portfolio_popup"
                    href="https://github.com/weialdin/backend_Weicommerce"
                  >
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div
                      class="main"
                      data-img-url="/img/portfolio/backend.png"
                    ></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>WeiCommerce Backend</h3>
                  <span>Ecommerce</span>
                </div>
              </div>
            </li>
          </ul>
        </div>
      </div>
      <div class="brush_1 wow zoomIn" data-wow-duration="1s">
        <img src="/img/brushes/portfolio/1.png" alt="" />
      </div>
      <div class="brush_2 wow fadeInRight" data-wow-duration="1s">
        <img src="/img/brushes/portfolio/2.png" alt="" />
      </div>
    </div>
  </div>
  <MagnificPopUpVue
    :modal="modal"
    :close="closeModal"
    :name="name"
    :src="src"
  />
  <div :class="`${active === 1 ? '' : 'hidden_content'}`">
    <ModalBox :close="close">
      <div class="popup_details">
        <div class="top_image">
          <img src="img/thumbs/4-2.jpg" alt="" />
          <div
            class="main"
            data-img-url="img/portfolio/6.jpg"
            style="background-image: url('img/portfolio/6.jpg')"
          ></div>
        </div>
        <div class="portfolio_main_title">
          <h3>Global Evolution</h3>
          <span><a href="#">Detail</a></span>
          <div></div>
        </div>
        <div class="main_details">
          <div class="textbox">
            <p>
              We live in a world where we need to move quickly and iterate on
              our ideas as flexibly as possible.
            </p>
            <p>
              Mockups are useful both for the creative phase of the project -
              for instance when you're trying to figure out your user flows or
              the proper visual hierarchy - and the production phase when they
              phase when they will represent the target product. Building
              mockups strikes the ideal balance ease of modification.
            </p>
          </div>
          <div class="detailbox">
            <ul>
              <li>
                <span class="first">Client</span>
                <span>Alvaro Morata</span>
              </li>
              <li>
                <span class="first">Category</span>
                <span><a href="#">Detail</a></span>
              </li>
              <li>
                <span class="first">Date</span>
                <span>March 07, 2021</span>
              </li>
            </ul>
          </div>
        </div>
        <div class="additional_images">
          <ul>
            <li>
              <div class="list_inner">
                <div class="my_image">
                  <img src="img/thumbs/4-2.jpg" alt="" />
                  <div
                    class="main"
                    data-img-url="img/portfolio/1.jpg"
                    style="background-image: url('img/portfolio/1.jpg')"
                  ></div>
                </div>
              </div>
            </li>
            <li>
              <div class="list_inner">
                <div class="my_image">
                  <img src="img/thumbs/4-2.jpg" alt="" />
                  <div
                    class="main"
                    data-img-url="img/portfolio/2.jpg"
                    style="background-image: url('img/portfolio/2.jpg')"
                  ></div>
                </div>
              </div>
            </li>
            <li>
              <div class="list_inner">
                <div class="my_image">
                  <img src="img/thumbs/4-2.jpg" alt="" />
                  <div
                    class="main"
                    data-img-url="img/portfolio/3.jpg"
                    style="background-image: url('img/portfolio/3.jpg')"
                  ></div>
                </div>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </ModalBox>
  </div>
</template>

<script>
import MagnificPopUpVue from "./popup/MagnificPopUp.vue";
import ModalBox from "./popup/ModalBox.vue";
export default {
  name: "PortfolioComponent",
  data() {
    return {
      activeNav: "1", // props
      name: "",
      src: "",
      modal: false,
      // Content
      active: 0,
    };
  },
  mounted() {
    let Isotope = require("isotope-layout");
    setTimeout(() => {
      let iso = new Isotope(".gallery_zoom", {
        itemSelector: ".grid-item",
        //    layoutMode: "fitRows",
        percentPosition: true,
        masonry: {
          columnWidth: ".grid-item",
        },
        animationOptions: {
          duration: 750,
          easing: "linear",
          queue: false,
        },
      });
      let filterFns = {
        // show if number is greater than 50
        numberGreaterThan50: function (itemElem) {
          let number = itemElem.querySelector(".number").textContent;
          return parseInt(number, 10) > 50;
        },
        // show if name ends with -ium
        ium: function (itemElem) {
          let name = itemElem.querySelector(".name").textContent;
          return name.match(/ium$/);
        },
      };
      // bind filter button click filter main funtion
      let filtersElem = document.querySelector(".portfolio_filter ul");
      filtersElem.addEventListener("click", function (event) {
        if (event.target.getAttribute("data-filter")) {
          let filterValue = event.target.getAttribute("data-filter");
          filterValue = filterFns[filterValue] || filterValue;
          iso.arrange({ filter: filterValue });
        }
      });
    }, 1000);
  },
  methods: {
    onClick(name, src) {
      this.name = name;
      this.src = src;
      this.modal = true;
    },
    closeModal() {
      this.modal = false;
      this.name = "";
      this.src = "";
    },
    close() {
      this.active = 0;
    },
  },
  components: { MagnificPopUpVue, ModalBox },
};
</script>
