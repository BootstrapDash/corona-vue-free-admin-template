<template>
  <section class="app-sidebar">
    <nav class="sidebar sidebar-offcanvas" id="sidebar">
      <div class="sidebar-brand-wrapper d-none d-lg-flex align-items-center justify-content-center fixed-top text-center">
        <router-link class="sidebar-brand brand-logo" to="/">
          <img src="@/assets/images/logo.svg" alt="logo" />
        </router-link>
        <router-link class="sidebar-brand brand-logo-mini" to="/">
          <img src="@/assets/images/logo-mini.svg" alt="logo" />
        </router-link>
      </div>
      <ul class="nav">
        <li class="nav-item account-dropdown">
          <a class="nav-link" v-b-toggle="'account-dropdown'">
            <img class="img-xs rounded-circle" src="@/assets/images/faces-clipart/pic-1.png" alt="">
            <p class="mb-0 text-light">Stella Johnson</p>
            <i class="menu-arrow"></i>
          </a>
          <b-collapse accordion="sidebar-accordion" id="account-dropdown">
            <ul class="nav flex-column sub-menu pl-0">
              <li class="nav-item">
                <a class="nav-link pl-5" href="#">
                  <span class="menu-icon">
                    <i class="mdi mdi-account"></i>
                  </span>
                  <span class="menu-title">Profile</span>
                </a>
              </li>
              <li class="nav-item">
                <a class="nav-link pl-5" href="#">
                  <span class="menu-icon">
                    <i class="mdi mdi-email"></i>
                  </span>
                  <span class="menu-title">Inbox</span>
                </a>
              </li>
              <li class="nav-item">
                <a class="nav-link pl-5" href="#">
                  <span class="menu-icon">
                    <i class="mdi mdi-wrench"></i>
                  </span>
                  <span class="menu-title">Settings</span>
                </a>
              </li>
              <li class="nav-item">
                <a class="nav-link pl-5" href="#">
                  <span class="menu-icon">
                    <i class="mdi mdi-power"></i>
                  </span>
                  <span class="menu-title">Logout</span>
                </a>
              </li>
            </ul>
          </b-collapse>
        </li>
        <li class="nav-item nav-category">
           <span class="nav-link">Navigation</span>
        </li>
        <li class="nav-item menu-items" v-on:click="collapseAll">
          <router-link class="nav-link" to="/">
            <span class="menu-icon">
              <i class="mdi mdi-speedometer"></i>
            </span>
            <span class="menu-title">Dashboard</span>
          </router-link>
        </li>
        <li class="nav-item menu-items">
          <span class="nav-link" v-b-toggle="'ui-basic'" :class="{'active': subIsActive('/basic-ui')}">
            <span class="menu-icon">
              <i class="mdi mdi-laptop"></i>
            </span>
            <span class="menu-title">Basic UI Elements</span>
            <i class="menu-arrow"></i>
          </span>
          <b-collapse accordion="sidebar-accordion" id="ui-basic">
            <ul class="nav flex-column sub-menu">
              <li class="nav-item">
                <router-link class="nav-link" to="/basic-ui/buttons/">Buttons</router-link>
              </li>
              <li class="nav-item">
                <router-link class="nav-link" to="/basic-ui/dropdowns/">Dropdowns</router-link>
              </li>
              <li class="nav-item">
                <router-link class="nav-link" to="/basic-ui/typography/">Typography</router-link>
              </li>
            </ul>
          </b-collapse>
        </li>
        <li class="nav-item menu-items">
          <span class="nav-link" v-b-toggle="'charts-dropdown'" :class="{'active': subIsActive('/charts')}">
            <span class="menu-icon">
              <i class="mdi mdi-chart-bar"></i>
            </span>
            <span class="menu-title">Charts</span>
            <i class="menu-arrow"></i>
          </span>
          <b-collapse accordion="sidebar-accordion" id="charts-dropdown">
            <ul class="nav flex-column sub-menu">
              <li class="nav-item">
                <router-link class="nav-link" to="/charts/chartjs/">ChartJS</router-link>
              </li>
            </ul>
          </b-collapse>
        </li>
        <li class="nav-item menu-items">
          <span class="nav-link" v-b-toggle="'table-dropdown'" :class="{'active': subIsActive('/tables')}">
            <span class="menu-icon">
              <i class="mdi mdi-table-large"></i>
            </span>
            <span class="menu-title">Tables</span>
            <i class="menu-arrow"></i>
          </span>
          <b-collapse accordion="sidebar-accordion" id="table-dropdown">
            <ul class="nav flex-column sub-menu">
              <li class="nav-item">
                <router-link class="nav-link" to="/tables/basic-tables/">Basic Table</router-link>
              </li>
            </ul>
          </b-collapse>
        </li>
        <li class="nav-item menu-items">
          <span class="nav-link" v-b-toggle="'user-page-dropdown'" :class="{'active': subIsActive('/auth-pages')}">
            <span class="menu-icon">
              <i class="mdi mdi-security"></i>
            </span>
            <span class="menu-title">User Pages</span>
            <i class="menu-arrow"></i>
          </span>
          <b-collapse accordion="sidebar-accordion" id="user-page-dropdown">
            <ul class="nav flex-column sub-menu">
              <li class="nav-item">
                <router-link class="nav-link" to="/auth-pages/login/">Login</router-link>
              </li>
              <li class="nav-item">
                <router-link class="nav-link" to="/auth-pages/register/">Register</router-link>
              </li>
            </ul>
          </b-collapse>
        </li>
        <li class="nav-item menu-items">
          <span class="nav-link" v-b-toggle="'error-page-dropdown'" :class="{'active': subIsActive('/error-pages')}">
            <span class="menu-icon">
              <i class="mdi mdi-lock"></i>
            </span>
            <span class="menu-title">Error pages</span>
            <i class="menu-arrow"></i>
          </span>
          <b-collapse accordion="sidebar-accordion" id="error-page-dropdown">
            <ul class="nav flex-column sub-menu">
              <li class="nav-item">
                <router-link class="nav-link" to="/error-pages/error-404/">404</router-link>
              </li>
              <li class="nav-item">
                <router-link class="nav-link" to="/error-pages/error-500/">500</router-link>
              </li>
            </ul>
          </b-collapse>
        </li>
        <li class="nav-item menu-items">
          <span class="nav-link" v-b-toggle="'form-elements'" :class="{'active': subIsActive('/forms')}">
            <span class="menu-icon">
              <i class="mdi mdi-playlist-play"></i>
            </span>
            <span class="menu-title">Forms</span>
            <i class="menu-arrow"></i>
          </span>
          <b-collapse accordion="sidebar-accordion" id="form-elements">
            <ul class="nav flex-column sub-menu">
              <li class="nav-item">
                <router-link class="nav-link" to="/forms/basic-elements/">Basic Elements</router-link>
              </li>
            </ul>
          </b-collapse>
        </li>
        <li class="nav-item menu-items">
          <span class="nav-link" v-b-toggle="'icons-dropdown'" :class="{'active': subIsActive('/icons')}">
            <span class="menu-icon">
              <i class="mdi mdi-contacts"></i>
            </span>
            <span class="menu-title">Icons</span>
            <i class="menu-arrow"></i>
          </span>
          <b-collapse accordion="sidebar-accordion" id="icons-dropdown">
            <ul class="nav flex-column sub-menu">
               <li class="nav-item">
                <router-link class="nav-link" to="/icons/mdi-icons/">MDI</router-link>
              </li>
            </ul>
          </b-collapse>
        </li>
        <li class="nav-item menu-items" v-on:click="collapseAll">
          <a class="nav-link" target="_blank" href="http://www.bootstrapdash.com/demo/corona-vue-free/documentation/documentation.html">
            <span class="menu-icon">
              <i class="mdi mdi-file-document-box"></i>
            </span>
            <span class="menu-title">Documentation</span>
          </a>
        </li>
      </ul>
    </nav>
  </section>
</template>

<script>
export default {
  name: 'sidebar',
 data () {
    return {
      collapses: [ 
     { show: false },
     { show: false },
     { show: false }
    ]
    }
  },

  mounted () {
    const body = document.querySelector('body')
    // add class 'hover-open' to sidebar navitem while hover in sidebar-icon-only menu
    document.querySelectorAll('.sidebar .nav-item').forEach(function (el) {
      el.addEventListener('mouseover', function () {
        if (body.classList.contains('sidebar-icon-only')) {
          el.classList.add('hover-open')
        }
      })
      el.addEventListener('mouseout', function () {
        if (body.classList.contains('sidebar-icon-only')) {
          el.classList.remove('hover-open')
        }
      })
    })
    
  },
  methods: {
    collapseAll() {
      var exp_element = document.getElementsByClassName("show");
      if (exp_element.length > 0) {
        var elm_id = exp_element[0].id;
        this.$root.$emit("bv::toggle::collapse", elm_id);
      }
    },
    subIsActive(input) {
    const paths = Array.isArray(input) ? input : [input]
    return paths.some(path => {
      return this.$route.path.indexOf(path) === 0 // current path starts with this path string
    })
  }
  },
  watch:{
    $route () {
       document.querySelector('#sidebar').classList.toggle('active');
    }
  } 
}
</script>