<template>
  <div>
    <header class="nav-opt-sprite nav-locate-us nav-lang-en nav-ssl nav-unrec">
      <div class="container-fluid desktop-nav">
        <div class="row">
          <!-- Logo -->
          <div class="col-sm-2">
            <div class="logo-area">
              <a href="#">
                <img src="/img/logo.png" alt="logo" class="img-fluid" />
              </a>
            </div>
          </div>
          <!-- Search bar -->
          <div class="col-sm-6 pt-0">
            <Search />
          </div>
          <div class="col-sm-4"></div>
        </div>

        <div class="row">
          <!-- Delivery -->
          <div class="col-lx-2 col-lg-2 col-md-2 col-sm-2 pl-2">
            <div class="nav-global-location">
              <nuxt-link to="/address" class="nav-a nav-a-2">
                <div class="nav-sprite" id="nav-packard-glow-loc-icon"></div>
                <div id="glow-ingress-block">
                  <span class="nav-line-1" id="glow-ingress-line1"
                    >Deliver to</span
                  >
                  <span class="nav-line-2" id="glow-ingress-line2"
                    >California</span
                  >
                </div>
              </nuxt-link>
            </div>
          </div>

          <!-- Shopping -->
          <div class="col-xl-6 col-lg-5 col-md-4 col-sm-6 p-0">
            <div class="nav-fill">
              <div class="nav-shop">
                <nuxt-link
                  to="/history"
                  class="nav-a nav-a-2 nav-single-row-link"
                >
                  <span class="nav-line-2">
                    Browsing history
                    <span
                      class="nav-icon nav-arrow"
                      style="visibility: visible"
                    ></span>
                  </span>
                </nuxt-link>
              </div>

              <div class="nav-xshop-container">
                <div class="nav-xshop">
                  <a href="#" class="nav-a">Today's deals</a>
                  <a href="#" class="nav-a">Your shop</a>
                  <a href="#" class="nav-a">Gift cards</a>
                  <a href="#" class="nav-a">Registry</a>
                  <a href="#" class="nav-a">Sell</a>
                </div>
              </div>
            </div>
          </div>

          <!-- Accounts, order and cart -->
          <div class="col-xl-4 col-lg-5 col-md-6 col-sm-4 p-0">
            <div class="nav-tools">
              <a
                href="#"
                id="icp-nav-flyout"
                class="nav-a nav-a-2 icp-link-style-2"
              >
                <span class="icp-nav-link-inner">
                  <span class="nav-line-1">
                    <span class="icp-nav-globe-img-2"></span>
                    <span class="icp-nav-language">EN</span>
                  </span>

                  <span class="nav-line-2">
                    &nbsp;
                    <span
                      class="nav-icon nav-arrow"
                      style="visibility: visible"
                    ></span>
                  </span>
                </span>
              </a>
              <span class="icp-nav-link-border"></span>
              <nuxt-link
                to="/register"
                class="nav-a nav-a-2"
                id="nav-link-accountList"
                tabindex="0"
              >
                <span class="nav-line-1">Hello, Sign in</span>
                <span class="nav-line-2">
                  Account &amp; Lists
                  <span
                    class="nav-icon nav-arrow"
                    style="visibility: visible"
                  ></span>
                </span>
              </nuxt-link>
              <nuxt-link to="/orders" class="nav-a nav-a-2 nav-single-row-link">
                <span class="nav-line-1"></span>
                <span class="nav-line-2">Orders</span>
              </nuxt-link>
              <nuxt-link to="/cart" class="nav-a nav-a-2" id="nav-cart">
                <span aria-hidden="true" class="nav-line-1"></span>
                <span aria-hidden="true" class="nav-line-2">Cart</span>
                <span class="nav-cart-icon nav-sprite"></span>
                <span
                  id="nav-cart-count"
                  aria-hidden="true"
                  class="nav-cart-count nav-cart-0"
                  >0</span
                >
              </nuxt-link>
            </div>
          </div>
        </div>
      </div>
    </header>
  </div>
</template>

<script>
import Search from "~/components/Search";

export default {
  components: {
    Search,
  },
};
</script>

<style>
</style>