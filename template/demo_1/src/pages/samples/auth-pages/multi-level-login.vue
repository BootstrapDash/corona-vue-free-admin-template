<template>

  <section class="multi-level-login">
    <div class="container-scroller">
      <div class="container-fluid page-body-wrapper full-page-wrapper">
        <div class="content-wrapper">
          <div class="multi-level-login">
            <div class="row">
              <div class="col-12 col-lg-7 mx-auto">
                <h3 class="text-center mb-5">Create your account</h3>
                <vue-good-wizard :steps="steps" :onNext="nextClicked" :onBack="backClicked">
                  <div slot="page1">
                    <div class="form-group">
                      <input class="form-control" type="text" name="username" placeholder="Username" />
                    </div>
                    <div class="form-group">
                      <input class="form-control" type="password" name="pass" placeholder="Password" />
                    </div>
                    <div class="form-group">
                      <input class="form-control" type="password" name="cpass" placeholder="Confirm Password" />
                    </div>
                  </div>
                  <div slot="page2">
                    <div class="row">
                      <div class="form-group col-md-6">
                        <input class="form-control" type="text" name="FirstName" placeholder="First Name" />
                      </div>
                      <div class="form-group col-md-6">
                        <input class="form-control" type="text" name="Last Name" placeholder="Last Name" />
                      </div>
                    </div>
                    <div class="row">
                      <div class="form-group col-md-6">
                        <input class="form-control" type="email" name="email" placeholder="Email" />
                      </div>
                      <div class="form-group col-md-6">
                        <input class="form-control" type="text" name="Country" placeholder="Country" />
                      </div>
                    </div>
                    <div class="form-group">
                      <input class="form-control" type="number" name="Number" placeholder="Number" />
                    </div>
                  </div>
                  <div slot="page3">
                    <div class="text-center">
                      <p class="font-weight-bold">Created sucessfully</p>
                      <i class="mdi mdi-shield-check text-warning icon-lg"></i>
                      <h4 class="font-weight-bold">Welcome staradmin</h4>
                      <p class="mb-0 text-muted">You’ve successfully created a account for this user.</p>
                    </div>
                  </div>
                </vue-good-wizard>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    
  </section>

</template>

<script>
import { GoodWizard } from 'vue-good-wizard'
export default {
  name: 'wizard',
  components: {
    'vue-good-wizard': GoodWizard
  },
  data () {
    return {
      steps: [
        {
          label: 'Login details',
          slot: 'page1'
        },
        {
          label: 'User Profile',
          slot: 'page2'
        },
        {
          label: 'Finish',
          slot: 'page3'
        }
      ]
    }
  },
  methods: {
    nextClicked () {
      return true
    },
    backClicked () {
      return true
    }
  }
}
</script>
