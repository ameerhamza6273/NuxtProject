<template>
  <v-app>
    <v-app-bar app flat class="app-bar-style px-lg-15 px-md-5 px-sm-10 elevation-2" height="90" color="white">
      <!-- app bar logo is here -->
      <div>
        <img alt="Vuetify Logo" src="../assets/logo_ambar (1).svg" width="165" style="cursor: pointer;" @click="Ammbar"/>
      </div>
      <v-spacer></v-spacer>
      <!-- app bar links is here -->
      <router-link 
      v-for="item in menubarTitle" 
      :key="item.title" 
      :to="item.path"
        class="d-none d-md-block router-link-style"
        >
        <v-btn text color="#EBF7FB" class="router-style rounded-0" height="90px">
          <span class="links-style">{{ item.title }}</span>
        </v-btn>
      </router-link>

      <v-spacer></v-spacer>
      <!-- app bar login btn is here -->
      <v-btn class="login-btn d-none d-sm-flex rounded-lg white--text" depressed color="#041E42" style="height: 50px !important;"><span>Log in</span></v-btn>
      <v-app-bar-nav-icon class="d-md-none" size="60" @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
    </v-app-bar>
    <!-- navigation drawer is here -->
    <v-navigation-drawer v-model="drawer" right app temporary style="background-color: #FFF ;">
      <v-list-item style="background-color: #041e42e7 ;">
        <v-list-item-content>
          <v-list-item-title>
            <img src="../assets/Vector (1).png" alt="user" width="10px" class="ml-7">
            <img src="../assets/Vector (2).png" alt="user" width="20px" class="ml-8">
            <img src="../assets/instagram.png" alt="user" width="17px" class="ml-8">
            <img src="../assets/whatsapp.png" alt="user" width="20px" class="ml-8">
          </v-list-item-title>
        </v-list-item-content>
      </v-list-item>
      <v-divider></v-divider>
      <v-list dense nav>
        <v-list-item 
        v-for="item in menubarTitle" 
        :key="item.title" link 
        :to="item.path" 
        style="color: black;"
        >
          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <v-btn class="login-btn d-sm-none d-md-flex px-6 ml-4 rounded-lg white--text" depressed color="#041E42" style="height: 40px !important;"><span>Log in</span></v-btn>
    </v-navigation-drawer>
    <v-main style="background-color: transparent;">
      <router-view />
    </v-main>
    <!-- footer is here -->
    <AmbarFotr/>
  </v-app>
</template>

<script>
import AmbarFotr from '~/components/AmbarFotr.vue';
export default {
  name: "App",
  components: {
    AmbarFotr,
  },
  data: () => ({
    pageTitle: 'Ambar Immigration',
    drawer: false,
    // links and path array
    menubarTitle: [
      { title: 'Home', path: "/" },
      { title: 'EB-3 Process', path: "/process" },
      { title: 'Jobs', path: "/jobs" },
      { title: 'Check Eligibility', path: "/eligibility" },
      { title: 'Employer Services', path: "/employerServices" },
      { title: 'Contact Us', path: "/contactUs" },
    ],
    // meta: [
    //     {
    //     title: 'index page title',
    //     name: 'discription detail test data',
    //     content: 'xyzz conteeeeeeeeeeeeeeeeee',
    //   }
    // ]
  }),
  mounted() {
        document.title = this.pageTitle;
    },
  methods: {
    Ammbar() {
      this.$router.push("/ambar");
    }
  },

};
</script>
<style>

.mdi-menu::before{
  color: black;
}
/* app bar links style */

.router-link-style {
  text-decoration: none !important;
}

.router-style .links-style {
  font-family: 'Poppins';
  font-style: normal;
  font-weight: 300;
  font-size: 14px;
  line-height: 24px;
  color: #111827;
  text-transform: capitalize;
  text-decoration: none !important;
}

/* app bar login btn style */
.login-btn {
  font-family: 'Poppins';
  font-style: normal;
  font-weight: 500;
  font-size: 15px;
  line-height: 24px;
  padding: 19px 32px !important;
}

/* active link style */
.nuxt-link-exact-active .router-style {
  background-color: rgba(4, 30, 66, 0.1);
  border-bottom: 2px solid #041E42 !important;
  font-weight: 800;
  color: #041E42 !important;
}

/* media queries is here */

@media screen and (max-width:1200px) {
  .router-style .links-style {
    font-weight: 300;
    font-size: 12px;
  }
}

@media screen and (max-width:1050px) {
  .router-style {
    padding: 7px !important;
  }

  .router-style .links-style {
    font-size: 11px;
  }
}
</style></style>


