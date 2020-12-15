<template>
  <b-navbar id="template-header" class="p-0 fixed-top d-flex flex-row" toggleable="lg">
    <div class="navbar-brand-wrapper d-flex d-lg-none align-items-center justify-content-center">
      <router-link class="navbar-brand brand-logo-mini" to="/">
        <img src="@/assets/images/logo-mini.svg" alt="logo" />
      </router-link>
    </div>
    <div class="navbar-menu-wrapper d-flex align-items-center ml-auto ml-lg-0">
      <button class="navbar-toggler navbar-toggler align-self-center d-lg-block" type="button" @click="toggleSidebar()">
        <span class="mdi mdi-format-line-spacing"></span>
      </button>
      <ul class="navbar-nav w-100">
        <li class="nav-item w-100">
          <form class="nav-link mt-2 mt-md-0 d-none d-lg-flex search">
            <input type="text" class="form-control" placeholder="Search Here..">
          </form>
        </li>
      </ul>
      <b-navbar-nav class="navbar-nav-right ml-auto">
        <b-nav-item-dropdown right class="preview-list">
          <template slot="button-content">
            <div class="count-indicator">
              <i class="mdi mdi-email"></i>
              <span class="count-symbol bg-danger">5</span>
            </div>
          </template>
          <h6 class="p-3 mb-0">Messages</h6>
          <b-dropdown-item class="preview-item">
            <div class="preview-thumbnail">
              <img src="@/assets/images/faces/face1.jpg" alt="image" class="profile-pic rounded-circle">
            </div>
            <div class="preview-item-content d-flex align-items-start flex-column justify-content-center">
              <p class="preview-subject ellipsis mb-1 font-weight-normal">Cregh send you a message</p>
              <p class="text-gray mb-0">15 Minutes ago</p>
            </div>
          </b-dropdown-item>
          <b-dropdown-item class="preview-item">
            <div class="preview-thumbnail">
              <img src="@/assets/images/faces/face2.jpg" alt="image" class="profile-pic rounded-circle">
            </div>
            <div class="preview-item-content d-flex align-items-start flex-column justify-content-center">
              <p class="preview-subject ellipsis mb-1 font-weight-normal">Profile picture updated</p>
              <p class="text-gray mb-0">18 Minutes ago</p>
            </div>
          </b-dropdown-item>
          <b-dropdown-item class="preview-item">
            <div class="preview-thumbnail">
              <img src="@/assets/images/faces/face3.jpg" alt="image" class="profile-pic rounded-circle">
            </div>
            <div class="preview-item-content d-flex align-items-start flex-column justify-content-center">
              <p class="preview-subject ellipsis mb-1 font-weight-normal">Mark send you a message</p>
              <p class="text-gray mb-0">1 Minutes ago</p>
            </div>
          </b-dropdown-item>
          <p class="p-3 mb-0 text-center border-top">4 new messages</p>
        </b-nav-item-dropdown>
        <b-nav-item-dropdown right class="preview-list border-left">
          <template slot="button-content">
            <div class="count-indicator">
              <i class="mdi mdi-bell"></i>
              <span class="count-symbol bg-danger">7</span>
            </div>
          </template>
          <h6 class="p-3 mb-0">Notifications</h6>
          <b-dropdown-item class="preview-item">
            <div class="preview-thumbnail">
              <div class="preview-icon bg-dark rounded-circle">
                <i class="mdi mdi-calendar text-success"></i>
              </div>
            </div>
            <div class="preview-item-content d-flex align-items-start flex-column justify-content-center">
              <p class="preview-subject font-weight-normal mb-1">Event today</p>
              <p class="text-gray ellipsis mb-0">
                Just a reminder that you have an event today
              </p>
            </div>
          </b-dropdown-item>
          <b-dropdown-item class="preview-item">
            <div class="preview-thumbnail">
              <div class="preview-icon bg-dark rounded-circle">
                <i class="mdi mdi-settings text-danger"></i>
              </div>
            </div>
            <div class="preview-item-content d-flex align-items-start flex-column justify-content-center">
              <p class="preview-subject font-weight-normal mb-1">Settings</p>
              <p class="text-gray ellipsis mb-0">
                Update dashboard
              </p>
            </div>
          </b-dropdown-item>
          <b-dropdown-item class="preview-item">
            <div class="preview-thumbnail">
              <div class="preview-icon bg-dark rounded-circle">
                <i class="mdi mdi-link-variant text-warning"></i>
              </div>
            </div>
            <div class="preview-item-content d-flex align-items-start flex-column justify-content-center">
              <p class="preview-subject font-weight-normal mb-1">Launch Admin</p>
              <p class="text-gray ellipsis mb-0">
                New admin wow!
              </p>
            </div>
          </b-dropdown-item>
          <p class="p-3 mb-0 text-center border-top">See all notifications</p>
        </b-nav-item-dropdown> 
        <b-nav-item-dropdown right class="preview-list nav-profile">
          <template slot="button-content">
            <div class="navbar-profile">
              <img class="img-xs rounded-circle" src="@/assets/images/faces-clipart/pic-1.png" alt="">
            </div> 
          </template>
        </b-nav-item-dropdown>
        <b-nav-item class="nav-logout d-none d-lg-block">
          <i class="mdi mdi-view-grid"></i>
        </b-nav-item>
      </b-navbar-nav>
      <button class="navbar-toggler navbar-toggler-right align-self-center" type="button" @click="toggleMobileSidebar()">
        <span class="mdi mdi-menu"></span>
      </button>
    </div>
  </b-navbar>
</template>

<script>
export default {
  name: 'app-header',
  methods: {
    toggleSidebar: () => {
      document.querySelector('body').classList.toggle('sidebar-icon-only');
    },
    toggleMobileSidebar: () => {
      document.querySelector('#sidebar').classList.toggle('active');
    }
  }
}
</script>

<style scoped>
</style>