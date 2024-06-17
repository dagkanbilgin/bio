<template>
  <div
    class="modal fade"
    id="exampleModalCenterportFolio2"
    tabindex="-1"
    role="dialog"
    aria-hidden="true"
  >
    <div class="modal-dialog modal-dialog-centered" role="document">
      <div class="modal-content">
        <div class="modal-header">
          <button
            type="button"
            class="close"
            data-bs-dismiss="modal"
            aria-label="Close"
          >
            <span aria-hidden="true"><i data-feather="x"></i></span>
          </button>
        </div>
        <div class="modal-body">
          <div class="row align-items-center">
            <div class="col-lg-6 portfolio-style-three">
              <div
                id="portfolio-modal-thumbnail-slider-63"
                style="position: relative"
              >
                <Swiper
                  :modules="[Navigation]"
                  :navigation="{
                    prevEl: '.snbpm1',
                    nextEl: '.snbnm1',
                  }"
                  :slides-per-view="1"
                  style="width: 100%"
                >
                  <SwiperSlide
                    v-for="(elm, i) in [1, 2, 3]"
                    :key="i"
                    class="swiper-slide"
                  >
                    <img
                      class="w-100 modal-portfolio-image"
                      :src="currentPortfolioModal.imgSrc"
                      alt="portfolio-large-05"
                    />
                  </SwiperSlide>
                </Swiper>
                <a class="carousel-control-prev snbpm1" role="button">
                  <span class="" aria-hidden="true">
                    <i class="feather-arrow-left"></i>
                  </span>
                  <span class="sr-only"></span>
                </a>
                <a class="carousel-control-next snbnm1" role="button">
                  <span class="" aria-hidden="true">
                    <i class="feather-arrow-right"></i>
                  </span>
                  <span class="sr-only"></span>
                </a>
              </div>
            </div>
            <div class="col-lg-6">
              <div class="text-content">
                <div class="row">
                  <div class="col-md-12">
                    <h3>{{ currentPortfolioModal.title }}</h3>
                    <p>
                      Through a wide variety of
                      <strong>mobile applications</strong>, we’ve developed a
                      unique visual system.
                    </p>
                    <div class="info-list">
                      <ul>
                        <li>
                          <strong>Client</strong> <span>George Wallace</span>
                        </li>
                        <li><strong>Date</strong> <span>15 June 2022</span></li>
                        <li>
                          <strong>Services</strong>
                          <span>Web Application </span>
                        </li>
                        <li><strong>Budget</strong> <span>$100000+</span></li>
                      </ul>
                    </div>
                  </div>
                  <div class="col-md-12">
                    <div class="button-group d-flex flex-wrap mt--20">
                      <div class="post-like pt-like-it">
                        <a
                          class="like-button rn-btn thumbs-icon rn-btn thumbs-icon"
                          href="https://themeforest.net/user/rainbow-themes"
                          data-id="63"
                          data-nonce="03eae30b94"
                        >
                          <span> LIKE THIS </span>
                          <i class="feather-thumbs-up mr--10"></i>
                          <mark id="like-count2-63" class="like-count badge">
                            {{ currentPortfolioModal.likes }}
                          </mark>
                        </a>
                      </div>
                      <a
                        href="https://themeforest.net/user/rainbow-themes"
                        class="rn-btn"
                        target="_blank"
                      >
                        <span>VIEW PROJECT</span>
                        <i class="feather-arrow-right-circle"></i
                      ></a>
                    </div>
                  </div>
                </div>
              </div>
              <!-- End of .text-content -->
            </div>
          </div>
          <!-- End of .row media-->
          <div class="row">
            <div class="col-md-12 portfolio-modal-info">
              <div class="pb--30 pt--55">
                <div class="section-separator w-100"></div>
              </div>

              <div class="row mt-5 mb-5">
                <p>
                  There are always some stocks, which illusively scale lofty
                  heights in a given time period. However, the good show doesn’t
                  last for these overblown toxic stocks as their current price
                  is not justified by their fundamental strength.
                </p>
                <div class="col-lg-4 col-md-6 col-sm-12">
                  <h5 class="portfolio-modal-h5"><strong>Strategy</strong></h5>
                  <p>
                    A strategy is a general plan to achieve one or more
                    long-term. labore et dolore magna aliqua.
                  </p>
                </div>
                <div class="col-lg-4 col-md-6 col-sm-12">
                  <h5 class="portfolio-modal-h5"><strong>Design</strong></h5>
                  <p>
                    UI/UX Design, Art Direction, A design is a plan or
                    specification for art. which illusively scale lofty heights.
                  </p>
                </div>
                <div class="col-lg-4 col-md-6 col-sm-12">
                  <h5 class="portfolio-modal-h5">
                    <strong>User Experience</strong>
                  </h5>
                  <p>
                    User experience (UX) design is the process design teams use
                    to create products that provide.
                  </p>
                </div>
              </div>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua. Quis
                ipsum suspendisse ultrices gravida. Risus commod viverra
                maecenas accumsan lacus vel facilisis. ut labore et dolore magna
                aliqua.
              </p>
              <p>
                However, if you can precisely spot such toxic stocks, you may
                gain by resorting to an investing strategy called short selling.
                This strategy allows one to sell a stock first and then buy it
                when the price falls.
              </p>
              <p>
                While short selling excels in bear markets, it typically loses
                money in bull markets.
              </p>
              <p>
                So, just like identifying stocks with growth potential,
                pinpointing toxic stocks and offloading them at the right time
                is crucial to guard one’s portfolio from big losses or make
                profits by short selling them. Heska Corporation HSKA, Tandem
                Diabetes Care, Inc.&nbsp;TNDM, Credit Suisse Group CS,Zalando SE
                ZLNDY and Las Vegas Sands LVS are a few such toxic
                stocks.Screening Criteria
              </p>
            </div>
          </div>

          <!-- End of .row body-->
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { Navigation } from "swiper/modules";
import { SwiperSlide } from "swiper/vue";
import { Swiper } from "swiper/vue";
import { currentPortfolioModal } from "~/context/modalContent";
</script>

<style lang="scss">
@import "swiper/css";
</style>
