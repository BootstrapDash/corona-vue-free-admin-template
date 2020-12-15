<template>

  <section class="buttons">
    <div class="page-header">
      <h3 class="page-title">
        Button
      </h3>
      <nav aria-label="breadcrumb">
        <ol class="breadcrumb">
          <li class="breadcrumb-item"><a href="javascript:void(0);">UI Elements</a></li>
          <li class="breadcrumb-item active" aria-current="page">Buttons</li>
        </ol>
      </nav>
    </div>
    <div class="row">
      <div class="col-12 grid-margin stretch-card">
        <div class="card">
          <div class="card-body">
            <h4 class="card-title">Normal buttons</h4>
            <p class="card-description">Add class <code>.btn-{color}</code> for buttons in theme colors</p>
            <div class="template-demo">
              <b-button variant="primary" class="btn-fw">Primary</b-button>
              <b-button variant="secondary" class="btn-fw">Secondary</b-button>
              <b-button variant="success" class="btn-fw">Success</b-button>
              <b-button variant="danger" class="btn-fw">Danger</b-button>
              <b-button variant="warning" class="btn-fw">Warning</b-button>
              <b-button variant="info" class="btn-fw">Info</b-button>
              <b-button variant="light" class="btn-fw">Light</b-button>
              <b-button variant="dark" class="btn-fw">Dark</b-button>
              <b-button class="btn-fw btn-link bg-transparent border-0">Link</b-button>
            </div>
          </div>
          <div class="card-body">
            <h4 class="card-title">Rounded buttons</h4>
            <p class="card-description">Add class <code>.btn-rounded</code></p>
            <div class="template-demo">
              <b-button variant="primary" class="btn-fw btn-rounded">Primary</b-button>
              <b-button variant="secondary" class="btn-fw btn-rounded">Secondary</b-button>
              <b-button variant="success" class="btn-fw btn-rounded">Success</b-button>
              <b-button variant="danger" class="btn-fw btn-rounded">Danger</b-button>
              <b-button variant="warning" class="btn-fw btn-rounded">Warning</b-button>
              <b-button variant="info" class="btn-fw btn-rounded">Info</b-button>
              <b-button variant="light" class="btn-fw btn-rounded">Light</b-button>
              <b-button variant="dark" class="btn-fw btn-rounded">Dark</b-button>
              <b-button class="btn-fw btn-rounded btn-link bg-transparent border-0">Link</b-button>
            </div>
          </div>
          <div class="card-body">
            <h4 class="card-title">Outlined buttons</h4>
            <p class="card-description">Add class <code>.btn-outline-{color}</code> for outline buttons</p>
            <div class="template-demo">
              <b-button variant="outline-primary" class="btn-fw">Primary</b-button>
              <b-button variant="outline-secondary" class="btn-fw">Secondary</b-button>
              <b-button variant="outline-success" class="btn-fw">Success</b-button>
              <b-button variant="outline-danger" class="btn-fw">Danger</b-button>
              <b-button variant="outline-warning" class="btn-fw">Warning</b-button>
              <b-button variant="outline-info" class="btn-fw">Info</b-button>
              <b-button variant="outline-light" class="btn-fw">Light</b-button>
              <b-button variant="outline-dark" class="btn-fw">Dark</b-button>
              <b-button class="btn-fw btn-link bg-transparent border-0">Link</b-button>
            </div>
          </div>
          <div class="card-body">
            <h4 class="card-title">Inverse buttons</h4>
            <p class="card-description">Add class <code>.btn-inverse-{color} for inverse buttons</code></p>
            <div class="template-demo">
              <b-button variant="inverse-primary" class="btn-fw">Primary</b-button>
              <b-button variant="inverse-secondary" class="btn-fw">Secondary</b-button>
              <b-button variant="inverse-success" class="btn-fw">Success</b-button>
              <b-button variant="inverse-danger" class="btn-fw">Danger</b-button>
              <b-button variant="inverse-warning" class="btn-fw">Warning</b-button>
              <b-button variant="inverse-info" class="btn-fw">Info</b-button>
              <b-button variant="inverse-light" class="btn-fw">Light</b-button>
              <b-button variant="inverse-dark" class="btn-fw">Dark</b-button>
              <b-button class="btn-fw btn-link bg-transparent border-0">Link</b-button>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-8 grid-margin stretch-card">
        <div class="card">
          <div class="card-body">
            <div class="row">
              <div class="col-md-7">
                <h4 class="card-title">Icon Buttons</h4>
                <p class="card-description">Add class <code>.btn-icon</code> for buttons with only icons</p>
                <div class="template-demo d-flex justify-content-between flex-nowrap">
                  <b-button variant="primary" class="btn-rounded btn-icon">
                    <i class="mdi mdi-home-outline"></i>
                  </b-button>
                  <b-button variant="dark" class="btn-rounded btn-icon">
                    <i class="mdi mdi-internet-explorer"></i>
                  </b-button>
                  <b-button variant="danger" class="btn-rounded btn-icon">
                    <i class="mdi mdi-email-open"></i>
                  </b-button>
                  <b-button variant="info" class="btn-rounded btn-icon">
                    <i class="mdi mdi-star"></i>
                  </b-button>
                  <b-button variant="success" class="btn-rounded btn-icon">
                    <i class="mdi mdi-map-marker"></i>
                  </b-button>
                </div>
                <div class="template-demo d-flex justify-content-between flex-nowrap">
                  <b-button variant="inverse-primary" class="btn-rounded btn-icon">
                    <i class="mdi mdi-home-outline"></i>
                  </b-button>
                  <b-button variant="inverse-dark" class="btn-icon">
                    <i class="mdi mdi-internet-explorer"></i>
                  </b-button>
                  <b-button variant="inverse-danger" class="btn-icon">
                    <i class="mdi mdi-email-open"></i>
                  </b-button>
                  <b-button variant="inverse-info" class="btn-icon">
                    <i class="mdi mdi-star"></i>
                  </b-button>
                  <b-button variant="inverse-success" class="btn-icon">
                    <i class="mdi mdi-map-marker"></i>
                  </b-button>
                </div>
                <div class="template-demo d-flex justify-content-between flex-nowrap mt-4">
                  <b-button variant="outline-secondary" class="btn-rounded btn-icon">
                    <i class="mdi mdi-heart-outline text-danger"></i>
                  </b-button>
                  <b-button variant="outline-secondary" class="btn-rounded btn-icon">
                    <i class="mdi mdi-music text-dark"></i>
                  </b-button>
                  <b-button variant="outline-secondary" class="btn-rounded btn-icon">
                    <i class="mdi mdi-star text-secondary"></i>
                  </b-button>
                  <b-button variant="outline-secondary" class="btn-rounded btn-icon">
                    <i class="mdi mdi-signal text-info"></i>
                  </b-button>
                  <b-button variant="outline-secondary" class="btn-rounded btn-icon">
                    <i class="mdi mdi-trending-up text-success"></i>
                  </b-button>
                </div>
                <div class="template-demo d-flex justify-content-between flex-nowrap">
                  <b-button variant="outline-secondary" class="btn-rounded btn-icon">
                    <i class="mdi mdi-heart-outline"></i>
                  </b-button>
                  <b-button variant="outline-secondary" class="btn-rounded btn-icon">
                    <i class="mdi mdi-music"></i>
                  </b-button>
                  <b-button variant="outline-secondary" class="btn-rounded btn-icon">
                    <i class="mdi mdi-star"></i>
                  </b-button>
                  <b-button variant="outline-secondary" class="btn-rounded btn-icon">
                    <i class="mdi mdi-signal"></i>
                  </b-button>
                  <b-button variant="outline-secondary" class="btn-rounded btn-icon">
                    <i class="mdi mdi-trending-up"></i>
                  </b-button>
                </div>
              </div>
              <div class="col-md-5">
                <h4 class="card-title">Button Size</h4>
                <p class="card-description">Use class <code>.btn-{size}</code></p>
                <div class="template-demo">
                  <b-button variant="outline-secondary" class="btn-lg">btn-lg</b-button>
                  <b-button variant="outline-secondary" class="btn-md">btn-md</b-button>
                  <b-button variant="outline-secondary" class="btn-sm">btn-sm</b-button>
                </div>
                <div class="template-demo mt-4">
                  <b-button variant="danger" class="btn-lg">btn-lg</b-button>
                  <b-button variant="success" class="btn-md">btn-md</b-button>
                  <b-button variant="primary" class="btn-sm">btn-sm</b-button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-4 grid-margin stretch-card">
        <div class="card">
          <div class="card-body">
            <h4 class="card-title">Block buttons</h4>
            <p class="card-description">Add class <code>.btn-block</code></p>
            <div class="template-demo">
              <b-button variant="info" class="btn-lg btn-block">Block buttons
                <i class="mdi mdi-menu float-right"></i>
              </b-button>
              <b-button variant="dark" class="btn-lg btn-block">Block buttons</b-button>
              <b-button variant="primary" class="btn-lg btn-block">
                <i class="mdi mdi-account"></i>
                Block buttons
              </b-button>
              <b-button variant="outline-secondary" class="btn-lg btn-block">Block buttons</b-button>
            </div>
          </div>
        </div>
      </div>
      <div class="col-12 grid-margin">
        <div class="card">
          <div class="card-body">
            <div class="row">
              <div class="col-md-6">
                <h4 class="card-title">Button groups</h4>
                <p class="card-description">Wrap a series of buttons with <code>.btn</code>
                  in <code>.btn-group</code></p>
                <div class="template-demo">
                  <div class="btn-group" role="group" aria-label="Basic example">
                    <b-button variant="outline-secondary">1</b-button>
                    <b-button variant="outline-secondary">2</b-button>
                    <b-button variant="outline-secondary">3</b-button>
                  </div>
                  <div class="btn-group" role="group" aria-label="Basic example">
                    <b-button variant="outline-secondary">
                      <i class="mdi mdi-heart-outline"></i>
                    </b-button>
                    <b-button variant="outline-secondary">
                      <i class="mdi mdi-calendar"></i>
                    </b-button>
                    <b-button variant="outline-secondary">
                      <i class="mdi mdi-clock"></i>
                    </b-button>
                  </div>
                </div>
                <div class="template-demo">
                  <div class="btn-group" role="group" aria-label="Basic example">
                    <b-button variant="primary">1</b-button>
                    <b-button variant="primary">2</b-button>
                    <b-button variant="primary">3</b-button>
                  </div>
                  <div class="btn-group" role="group" aria-label="Basic example">
                    <b-button variant="primary">
                      <i class="mdi mdi-heart-outline"></i>
                    </b-button>
                    <b-button variant="primary">
                      <i class="mdi mdi-calendar"></i>
                    </b-button>
                    <b-button variant="primary">
                      <i class="mdi mdi-clock"></i>
                    </b-button>
                  </div>
                </div>
                <div class="template-demo mt-4">
                  <div class="btn-group-vertical" role="group" aria-label="Basic example">
                    <b-button variant="outline-secondary">
                      <i class="mdi mdi-format-vertical-align-top"></i>
                    </b-button>
                    <b-button variant="outline-secondary">
                      <i class="mdi mdi-format-vertical-align-center"></i>
                    </b-button>
                    <b-button variant="outline-secondary">
                      <i class="mdi mdi-format-vertical-align-bottom"></i>
                    </b-button>
                  </div>
                  <div class="btn-group-vertical" role="group" aria-label="Basic example">
                    <b-button variant="outline-secondary">Default</b-button>
                    <div class="btn-group">
                      <b-button variant="outline-secondary" class="btn btn-outline-secondary dropdown-toggle" data-toggle="dropdown">Dropdown</b-button>
                      <div class="dropdown-menu">
                        <a class="dropdown-item">Go back</a>
                        <a class="dropdown-item">Delete</a>
                        <a class="dropdown-item">Swap</a>
                      </div>
                    </div>
                    <b-button variant="outline-secondary">Default</b-button>
                  </div>
                  <div class="btn-group-vertical" role="group" aria-label="Basic example">
                    <b-button variant="outline-secondary">Top</b-button>
                    <b-button variant="outline-secondary">Middle</b-button>
                    <b-button variant="outline-secondary">Bottom</b-button>
                  </div>
                </div>
                <div class="template-demo mt-4">
                  <div class="btn-group" role="group" aria-label="Basic example">
                    <b-button variant="outline-secondary">
                      <i class="mdi mdi-star d-block mb-1"></i>
                      Favourites
                    </b-button>
                    <b-button variant="outline-secondary">
                      <i class="mdi mdi-reload d-block mb-1"></i>
                      Reload
                    </b-button>
                    <b-button variant="outline-secondary">
                      <i class="mdi mdi-account d-block mb-1"></i>
                      Users
                    </b-button>
                  </div>
                </div>
              </div>
              <div class="col-md-6">
                <h4 class="card-title mt-4 mt-lg-0">Button with text and icon</h4>
                <p class="card-description">Wrap icon and text inside <code>.btn-icon-text</code> and use <code>.btn-icon-prepend</code>
                  or <code>.btn-icon-append</code> for icon tags</p>
                <div class="template-demo">
                  <b-button variant="primary" class="btn-icon-text">
                    <i class="mdi mdi-file-check btn-icon-prepend"></i>
                    Submit
                  </b-button>
                  <b-button variant="dark" class="btn-icon-text">
                    Edit
                    <i class="mdi mdi-file-check btn-icon-append"></i>
                  </b-button>
                  <b-button variant="success" class="btn-icon-text">
                    <i class="mdi mdi-alert btn-icon-prepend"></i>
                    Warning
                  </b-button>
                </div>
                <div class="template-demo">
                  <b-button variant="danger" class="btn-icon-text">
                    <i class="mdi mdi-upload btn-icon-prepend"></i>
                    Upload
                  </b-button>
                  <b-button variant="info" class="btn-icon-text">
                    Print
                    <i class="mdi mdi-printer btn-icon-append"></i>
                  </b-button>
                  <b-button variant="warning" class="btn-icon-text">
                    <i class="mdi mdi-reload btn-icon-prepend"></i>
                    Reset
                  </b-button>
                </div>
                <div class="template-demo mt-2">
                  <b-button variant="outline-primary" class="btn-icon-text">
                    <i class="mdi mdi-file-check btn-icon-prepend"></i>
                    Submit
                  </b-button>
                  <b-button variant="outline-secondary" class="btn-icon-text">
                    Edit
                    <i class="mdi mdi-file-check btn-icon-append"></i>
                  </b-button>
                  <b-button variant="outline-success" class="btn-icon-text">
                    <i class="mdi mdi-alert btn-icon-prepend"></i>
                    Warning
                  </b-button>
                </div>
                <div class="template-demo">
                  <b-button variant="outline-danger" class="btn-icon-text">
                    <i class="mdi mdi-upload btn-icon-prepend"></i>
                    Upload
                  </b-button>
                  <b-button variant="outline-info" class="btn-icon-text">
                    Print
                    <i class="mdi mdi-printer btn-icon-append"></i>
                  </b-button>
                  <b-button variant="outline-warning" class="btn-icon-text">
                    <i class="mdi mdi-reload btn-icon-prepend"></i>
                    Reset
                  </b-button>
                </div>
                <div class="template-demo mt-2">
                  <b-button variant="outline-secondary" class="btn-icon-text">
                    <i class="mdi mdi-apple btn-icon-prepend mdi-36px"></i>
                    <span class="d-inline-block text-left">
                      <small class="font-weight-light d-block">Available on the</small>
                      App Store
                    </span>
                  </b-button>
                  <b-button variant="outline-secondary" class="btn-icon-text">
                    <i class="mdi mdi-android-debug-bridge btn-icon-prepend mdi-36px"></i>
                    <span class="d-inline-block text-left">
                      <small class="font-weight-light d-block">Get it on the</small>
                      Google Play
                    </span>
                  </b-button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-6 grid-margin stretch-card">
        <div class="card">
          <div class="card-body">
            <h4 class="card-title">Social Icon Buttons</h4>
            <p class="card-description">Add class <code>.btn-social-icon</code></p>
            <div class="template-demo">
              <b-button variant="transparent" class="btn-social-icon btn-outline-facebook"><i class="mdi mdi-facebook"></i></b-button>
              <b-button variant="transparent" class="btn-social-icon btn-outline-youtube"><i class="mdi mdi-youtube"></i></b-button>
              <b-button variant="transparent" class="btn-social-icon btn-outline-twitter"><i class="mdi mdi-twitter"></i></b-button>
              <b-button variant="transparent" class="btn-social-icon btn-outline-dribbble"><i class="mdi mdi-dribbble"></i></b-button>
              <b-button variant="transparent" class="btn-social-icon btn-outline-linkedin"><i class="mdi mdi-linkedin"></i></b-button>
              <b-button variant="transparent" class="btn-social-icon btn-outline-google"><i class="mdi mdi-google-plus"></i></b-button>
            </div>
            <div class="template-demo">
              <b-button class="btn-social-icon btn-facebook border-0"><i class="mdi mdi-facebook"></i></b-button>
              <b-button class="btn-social-icon btn-youtube border-0"><i class="mdi mdi-youtube"></i></b-button>
              <b-button class="btn-social-icon btn-twitter border-0"><i class="mdi mdi-twitter"></i></b-button>
              <b-button class="btn-social-icon btn-dribbble border-0"><i class="mdi mdi-dribbble"></i></b-button>
              <b-button class="btn-social-icon btn-linkedin border-0"><i class="mdi mdi-linkedin"></i></b-button>
              <b-button class="btn-social-icon btn-google border-0"><i class="mdi mdi-google-plus"></i></b-button>
            </div>
            <div class="template-demo">
              <b-button class="btn-social-icon btn-facebook btn-rounded border-0"><i class="mdi mdi-facebook"></i></b-button>
              <b-button class="btn-social-icon btn-youtube btn-rounded border-0"><i class="mdi mdi-youtube"></i></b-button>
              <b-button class="btn-social-icon btn-twitter btn-rounded border-0"><i class="mdi mdi-twitter"></i></b-button>
              <b-button class="btn-social-icon btn-dribbble btn-rounded border-0"><i class="mdi mdi-dribbble"></i></b-button>
              <b-button class="btn-social-icon btn-linkedin btn-rounded border-0"><i class="mdi mdi-linkedin"></i></b-button>
              <b-button class="btn-social-icon btn-google btn-rounded border-0"><i class="mdi mdi-google-plus"></i></b-button>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-6 grid-margin stretch-card">
        <div class="card">
          <div class="card-body">
            <h4 class="card-title">Social button with text</h4>
            <p class="card-description">Add class <code>.btn-social-icon-text</code></p>
            <div class="template-demo">
              <b-button class="btn-social-icon-text btn-facebook border-0"><i class="mdi mdi-facebook"></i>Facebook</b-button>
              <b-button class="btn-social-icon-text btn-youtube border-0"><i class="mdi mdi-youtube"></i>Youtube</b-button>
              <b-button class="btn-social-icon-text btn-twitter border-0"><i class="mdi mdi-twitter"></i>Twitter</b-button>
              <b-button class="btn-social-icon-text btn-dribbble border-0"><i class="mdi mdi-dribbble"></i>Dribbble</b-button>
              <b-button class="btn-social-icon-text btn-linkedin border-0"><i class="mdi mdi-linkedin"></i>Linkedin</b-button>
              <b-button class="btn-social-icon-text btn-google border-0"><i class="mdi mdi-google-plus"></i>Google</b-button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

</template>

<script>
export default {
  name: 'buttons'
}
</script>