<template>
  <footer>
    <div class="footer">
      <div class="container">
        <div class="nav-footer">
          <ul class="nav-footer__menu">
            <li class="nav-footer__item" v-for="link in links" :key="link.alias">
              <router-link class="nav-footer__link" :to="link.url">{{ link.title }}</router-link>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
import { links } from '@/_config'

export default {
  data() {
    return {
      links: links
    }
  }
}
</script>
