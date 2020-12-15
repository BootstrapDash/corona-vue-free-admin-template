<template>
  <section class="dashboard">
    <div class="proBanner">
      <div>
        <span class="d-flex align-items-center purchase-popup">
          <p>Get tons of UI components, Plugins, multiple layouts, 20+ sample pages, and more!</p>
          <a href="https://www.bootstrapdash.com/product/corona-vue/?utm_source=organic&utm_medium=banner&utm_campaign=free-preview" rel="noopener noreferrer" target="_blank" class="btn btn-sm purchase-button btn-primary ml-auto">Check Pro Version</a>
          <i class="mdi mdi-close bannerClose"  @click="toggleProBanner()" ></i>
        </span>
      </div>
    </div>
    <div class="row">
      <div class="col-md-4 grid-margin stretch-card">
        <div class="card">
          <div class="card-body">
            <h4 class="card-title">Current Balance</h4>
            <radial-progress-bar class="ml-auto mr-auto demo-progress-circle" :diameter="200"
              :completed-steps="40"
              :total-steps="100"
              innerStrokeColor="#0c0c0c"
              startColor = "#d53f3a"
              stopColor="#d53f3a"
              :strokeWidth="20"
              >
            </radial-progress-bar>
            <div class="row my-1">
              <div class="col-lg-7 mx-auto text-center">
                <div id="currentBalanceCircle" class="progressbar-js-circle demo-progress-circle"></div>
                <h3 class="card-text mb-0 mt-4">360$</h3>
                <p class="card-text">Total Expense</p>
              </div>
            </div>
            <div class="row mt-3">
              <div class="col-12 bg-gray-dark d-flex flex-row py-3 px-4 rounded justify-content-between">
                <div>
                  <h6 class="mb-1">Transfer to stripe</h6>
                  <p class="card-text">Dec 25, 2018</p>
                </div>
                <div class="align-self-center">
                  <h6 class="font-weight-bold mb-0">650$</h6>
                </div>
              </div>
            </div>
            <div class="row mt-3">
              <div class="col-12 bg-gray-dark d-flex flex-row py-3 px-4 rounded">
                <div>
                  <h6 class="mb-1">Transfer to Paypal</h6>
                  <p class="card-text">Dec 31, 2018</p>
                </div>
                <div class="align-self-center flex-grow text-right">
                  <h6 class="font-weight-bold mb-0">530$</h6>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-8 grid-margin stretch-card">
        <div class="card">
          <div class="card-body">
            <div class="d-flex flex-row justify-content-between">
              <div>
                <h4 class="card-title">Open Projects</h4>
                <p>Your data status</p>
              </div>
              <div class="align-self-center">
                <p class="text-muted">View History</p>
              </div>
            </div>
            <div class="row">
              <div class="col-12">
                <div class="preview-list">
                  <div class="preview-item border-bottom  py-3">
                    <div class="preview-thumbnail">
                      <div class="preview-icon bg-primary rounded">
                        <i class="mdi mdi-file-document"></i>
                      </div>
                    </div>
                    <div class="preview-item-content d-sm-flex flex-grow">
                      <div class="flex-grow">
                        <h6 class="preview-subject">New Document</h6>
                        <p class="mb-0">Broadcast web app mockup</p>
                      </div>
                      <div class="mr-auto text-sm-right pt-2 pt-sm-0">
                        <p class="text-muted">15 minutes ago</p>
                        <p>30 tasks, 5 issues </p>
                      </div>
                    </div>
                  </div>
                  <div class="preview-item border-bottom  py-3">
                    <div class="preview-thumbnail">
                      <div class="preview-icon bg-success rounded">
                        <i class="mdi mdi-cloud-upload"></i>
                      </div>
                    </div>
                    <div class="preview-item-content d-sm-flex flex-grow">
                      <div class="flex-grow">
                        <h6 class="preview-subject">New Design</h6>
                        <p class="mb-0">Upload new design</p>
                      </div>
                      <div class="mr-auto text-sm-right pt-2 pt-sm-0">
                        <p class="text-muted">1 hour ago</p>
                        <p>23 tasks, 5 issues </p>
                      </div>
                    </div>
                  </div>
                  <div class="preview-item border-bottom  py-3">
                    <div class="preview-thumbnail">
                      <div class="preview-icon bg-info rounded">
                        <i class="mdi mdi-clock"></i>
                      </div>
                    </div>
                    <div class="preview-item-content d-sm-flex flex-grow">
                      <div class="flex-grow">
                        <h6 class="preview-subject">Project meeting</h6>
                        <p class="mb-0">New project discussion</p>
                      </div>
                      <div class="mr-auto text-sm-right pt-2 pt-sm-0">
                        <p class="text-muted">35 minutes ago</p>
                        <p>15 tasks, 2 issues </p>
                      </div>
                    </div>
                  </div>
                  <div class="preview-item border-bottom  py-3">
                    <div class="preview-thumbnail">
                      <div class="preview-icon bg-warning rounded">
                        <i class="mdi mdi-email"></i>
                      </div>
                    </div>
                    <div class="preview-item-content d-sm-flex flex-grow">
                      <div class="flex-grow">
                        <h6 class="preview-subject">Broadcast Mail</h6>
                        <p class="mb-0">Sent release details to team</p>
                      </div>
                      <div class="mr-auto text-sm-right pt-2 pt-sm-0">
                        <p class="text-muted">55 minutes ago</p>
                        <p>35 tasks, 7 issues </p>
                      </div>
                    </div>
                  </div>
                  <div class="preview-item py-3">
                    <div class="preview-thumbnail">
                      <div class="preview-icon bg-danger rounded">
                        <i class="mdi mdi-chart-pie"></i>
                      </div>
                    </div>
                    <div class="preview-item-content d-sm-flex flex-grow">
                      <div class="flex-grow">
                        <h6 class="preview-subject">Planning</h6>
                        <p class="mb-0">New application planning</p>
                      </div>
                      <div class="mr-auto text-sm-right pt-2 pt-sm-0">
                        <p class="text-muted">50 minutes ago</p>
                        <p>27 tasks, 4 issues </p>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-4 grid-margin stretch-card">
        <div class="card">
          <div class="card-body">
            <div class="d-flex flex-row p-3">
              <div class="align-self-top">
                <p class="card-title mb-1 font-weight-bold">Today's sales</p>
                <h3 class="mb-0">2800</h3>
              </div>
              <div class="align-self-center flex-grow text-right">
                <i class="icon-lg mdi mdi-chart-pie text-primary"></i>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-4 grid-margin stretch-card">
        <div class="card">
          <div class="card-body">
            <div class="d-flex flex-row p-3">
              <div class="align-self-top">
                <p class="card-title mb-1 font-weight-bold">Total Revenue</p>
                <h3 class="mb-0">38,879</h3>
              </div>
              <div class="align-self-center flex-grow text-right">
                <i class="icon-lg mdi mdi-cash-multiple text-warning"></i>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-4 grid-margin stretch-card">
        <div class="card">
          <div class="card-body">
            <div class="d-flex flex-row p-3">
              <div class="align-self-top">
                <p class="card-title mb-1 font-weight-bold">Today's Visits</p>
                <h3 class="mb-0">2569</h3>
              </div>
              <div class="align-self-center flex-grow text-right">
                <i class="icon-lg mdi mdi-account-outline text-success"></i>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-12 grid-margin">
        <div class="card">
          <div class="card-body">
            <h4 class="card-title">Order Status</h4>
            <div class="table-responsive">
              <table class="table">
                <thead>
                  <tr>
                    <th>
                      <div class="form-check m-0">
                        <label class="form-check-label">
                          <input class="checkbox" type="checkbox"><i class="input-helper"></i>
                        </label>
                      </div>
                    </th>
                    <th> Profile </th>
                    <th> Customer </th>
                    <th> Email </th>
                    <th> Products </th>
                    <th> Start Date </th>
                    <th> Actions </th>
                  </tr>
                </thead>
                <tbody>
                  <tr>
                    <td>
                      <div class="form-check m-0">
                        <label class="form-check-label">
                          <input class="checkbox" type="checkbox"><i class="input-helper"></i>
                        </label>
                      </div>
                    </td>
                    <td>
                      <img src="../../assets/images/faces/face1.jpg" alt="image" />
                    </td>
                    <td> David Grey </td>
                    <td> davidgrey@demo.com </td>
                    <td> 6300 </td>
                    <td> 01/11/2017 </td>
                    <td>
                      <i class="mdi mdi-pencil icon-sm mr-2 text-success"></i>
                      <i class="mdi mdi-close icon-sm text-danger"></i>
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <div class="form-check m-0">
                        <label class="form-check-label">
                          <input class="checkbox" type="checkbox"><i class="input-helper"></i>
                        </label>
                      </div>
                    </td>
                    <td>
                      <img src="../../assets/images/faces/face2.jpg" alt="image" />
                    </td>
                    <td> Stella Johnson </td>
                    <td> stella@demo.com </td>
                    <td> 1256 </td>
                    <td> 03/11/2017 </td>
                    <td>
                      <i class="mdi mdi-pencil icon-sm mr-2 text-success"></i>
                      <i class="mdi mdi-close icon-sm text-danger"></i>
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <div class="form-check m-0">
                        <label class="form-check-label">
                          <input class="checkbox" type="checkbox"><i class="input-helper"></i>
                        </label>
                      </div>
                    </td>
                    <td>
                      <img src="../../assets/images/faces/face5.jpg" alt="image" />
                    </td>
                    <td> Marina Michel </td>
                    <td> marinam@demo.com </td>
                    <td> 8600 </td>
                    <td> 26/10/2017 </td>
                    <td>
                      <i class="mdi mdi-pencil icon-sm mr-2 text-success"></i>
                      <i class="mdi mdi-close icon-sm text-danger"></i>
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <div class="form-check m-0">
                        <label class="form-check-label">
                          <input class="checkbox" type="checkbox"><i class="input-helper"></i>
                        </label>
                      </div>
                    </td>
                    <td>
                      <img src="../../assets/images/faces/face3.jpg" alt="image" />
                    </td>
                    <td> John Doe </td>
                    <td> djohn@demo.com </td>
                    <td> 3250 </td>
                    <td> 18/12/2017 </td>
                    <td>
                      <i class="mdi mdi-pencil icon-sm mr-2 text-success"></i>
                      <i class="mdi mdi-close icon-sm text-danger"></i>
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <div class="form-check m-0">
                        <label class="form-check-label">
                          <input class="checkbox" type="checkbox"><i class="input-helper"></i>
                        </label>
                      </div>
                    </td>
                    <td>
                      <img src="../../assets/images/faces/face4.jpg" alt="image" />
                    </td>
                    <td> Catherine </td>
                    <td> catherine@demo.com </td>
                    <td> 8750 </td>
                    <td> 15/09/2017 </td>
                    <td>
                      <i class="mdi mdi-pencil icon-sm mr-2 text-success"></i>
                      <i class="mdi mdi-close icon-sm text-danger"></i>
                    </td>
                  </tr>
                </tbody>
              </table>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6 stretch-card mb-4 mb-md-0">
        <div class="card">
          <div class="card-body">
            <h4 class="card-title">Messages</h4>
            <div class="preview-list">
              <div class="preview-item border-bottom  py-3">
                <div class="preview-thumbnail">
                  <img src="../../assets/images/faces/face6.jpg" alt="image" class="rounded-circle" />
                </div>
                <div class="preview-item-content d-flex flex-grow">
                  <div class="flex-grow">
                    <div class="d-sm-flex justify-content-between">
                      <h6 class="preview-subject">Richard Joy</h6>
                      <div class="d-flex">
                        <p class="text-small text-muted border-right pr-3">13.06.2017</p>
                        <p class="text-small text-muted pl-3">2 hours ago</p>
                      </div>
                    </div>
                    <p>Well, it seems to be working now. Thank You !</p>
                  </div>
                </div>
              </div>
              <div class="preview-item border-bottom  py-3">
                <div class="preview-thumbnail">
                  <img src="../../assets/images/faces/face8.jpg" alt="image" class="rounded-circle" />
                </div>
                <div class="preview-item-content d-flex flex-grow">
                  <div class="flex-grow">
                    <div class="d-sm-flex justify-content-between">
                      <h6 class="preview-subject">Richard Joy</h6>
                      <div class="d-flex">
                        <p class="text-small text-muted border-right pr-3">13.06.2017</p>
                        <p class="text-small text-muted pl-3">2 hours ago</p>
                      </div>
                    </div>
                    <p>Well, it seems to be working now. Thank You !</p>
                  </div>
                </div>
              </div>
              <div class="preview-item border-bottom  py-3">
                <div class="preview-thumbnail">
                  <img src="../../assets/images/faces/face9.jpg" alt="image" class="rounded-circle" />
                </div>
                <div class="preview-item-content d-flex flex-grow">
                  <div class="flex-grow">
                    <div class="d-sm-flex justify-content-between">
                      <h6 class="preview-subject">Richard Joy</h6>
                      <div class="d-flex">
                        <p class="text-small text-muted border-right pr-3">13.06.2017</p>
                        <p class="text-small text-muted pl-3">2 hours ago</p>
                      </div>
                    </div>
                    <p>Well, it seems to be working now. Thank You !</p>
                  </div>
                </div>
              </div>
              <div class="preview-item border-bottom  py-3">
                <div class="preview-thumbnail">
                  <img src="../../assets/images/faces/face11.jpg" alt="image" class="rounded-circle" />
                </div>
                <div class="preview-item-content d-flex flex-grow">
                  <div class="flex-grow">
                    <div class="d-sm-flex justify-content-between">
                      <h6 class="preview-subject">Richard Joy</h6>
                      <div class="d-flex">
                        <p class="text-small text-muted border-right pr-3">13.06.2017</p>
                        <p class="text-small text-muted pl-3">2 hours ago</p>
                      </div>
                    </div>
                    <p>Well, it seems to be working now. Thank You !</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-6 stretch-card">
        <div class="card">
          <div class="card-body">
            <h4 class="card-title">To do list</h4>
            <todoList></todoList>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import RadialProgressBar from 'vue-radial-progress'
import todoList from '../../components/apps/todoList'

export default {
  name: 'dashboard',
  components: {
    RadialProgressBar,
    todoList
  },
  data() {
    return {
      time1: null,
      slide1: 0,
    };
  },
  methods: {
    toggleProBanner: () => {
      document.querySelector('body').classList.toggle('pro-banner-collapse');
    }
  }
}
</script>

<style scoped>

</style>