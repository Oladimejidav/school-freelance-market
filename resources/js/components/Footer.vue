<template>
  <footer class="footer">
    <div class="footer__container">
      <div class="footer__description">
        <img src="/images/fav1.png" alt="">
        <p v-if="$matchMedia.xl">
         
        </p>
        <p v-if="$matchMedia.xl">
          USA,<br>
8 The Green Street A, Dover, DE 19901 <br>support@cheaprank.com
        </p>
      </div>

      <div class="footer__right">
        <div class="footer__right--top">
          <div class="footer-nav__section">
            <div class="footer-nav__menu">
              <div class="flex-row space-between w-100">
                <span>Company</span>
                <div v-if="!$matchMedia.xl">
                  <span class="iconify footer-nav__icon" data-icon="entypo:chevron-small-down" />
                </div>
              </div>
              <div v-if="$matchMedia.xl" class="footer-nav__menu--items">
                <div>About Us</div>
                <div>Careers</div>
                <div>Contact Us</div>
              </div>
            </div>
            <div class="footer-nav__menu">
              <div class="flex-row space-between w-100">
                <span>Further Information</span>
                <div v-show="!$matchMedia.xl">
                  <span class="iconify footer-nav__icon" data-icon="entypo:chevron-small-down" />
                </div>
              </div>
              <div v-show="$matchMedia.xl" class="footer-nav__menu--items">
                <div>Terms & Conditions</div>
                <div>Privacy Policy</div>
              </div>
            </div>
          </div>
          <div class="footer-icon__section">
            <div>Connect with us</div>
            <div class="footer-icon__container">
              <div>
                <span class="iconify footer-icon__item" data-icon="ant-design:instagram-outlined" />
              </div>
              <div>
                <span class="iconify footer-icon__item" data-icon="ant-design:twitter-outlined" />
              </div>
              <div>
                <span class="iconify footer-icon__item" data-icon="la:linkedin-in" />
              </div>
              <div>
                <span class="iconify footer-icon__item" data-icon="la:facebook-f" />
              </div>
            </div>
          </div>
        </div>

        <p class="footer__copyright">
           &copy; 2022 Cheaprank Inc. All Rights Reserved®
        </p>
      </div>
    </div>
  </footer>
</template>

<script>
import { mapGetters } from 'vuex'

export default {
  data: () => ({
    wishlists: '',
    searchQuery: ''
  }),

  computed: {
    ...mapGetters({
      // user: 'auth/user',
      // data: 'auth/data'
    })
  },

  mounted () {
    // this.getWishlist()
  },

  methods: {
    // async getWishlist () {
    //   this.wishlists = this.data.wishlists
    // }
  }
}
</script>
