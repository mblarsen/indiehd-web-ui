<template>
  <div class="section section-javascript" id="javascriptComponents">
    <div class="container">
      <h3 class="title">Javascript components</h3>
      <div class="row" id="modals">
        <div class="col-md-6 modal-buttons">
          <h4>Modal</h4>
          <n-button @click.native="modals.classic = true" type="primary">
            <i class="now-ui-icons files_single-copy-04"></i> Classic
          </n-button>
          <n-button @click.native="modals.mini = true" type="primary">
            <i class="now-ui-icons media-1_button-power"></i> Launch Modal Mini
          </n-button>
          <n-button @click.native="modals.notice = true" type="primary">
            <i class="now-ui-icons travel_info"></i> Notice
          </n-button>
          <n-button @click.native="modals.login = true" type="primary">
            <i class="now-ui-icons users_single-02"></i> Login Modal
          </n-button>
        </div>
        <div class="col-md-6 popover-buttons">
          <h4>Popovers</h4>
          <el-popover
              placement="left"
              popper-class="popover popover-primary"
              ref="popover1"
              trigger="hover"
              width="200">
            <h3 class="popover-header">Popover On Left</h3>
            <div class="popover-body">Here will be some very useful information about his popover.</div>
          </el-popover>

          <el-popover
              placement="top-start"
              popper-class="popover"
              ref="popover2"
              trigger="hover"
              width="200">
            <h3 class="popover-header">Popover On Top</h3>
            <div class="popover-body">Here will be some very useful information about his popover.</div>
          </el-popover>

          <el-popover
              placement="right"
              popper-class="popover"
              ref="popover3"
              trigger="hover"
              width="200">
            <h3 class="popover-header">Popover On Right</h3>
            <div class="popover-body">Here will be some very useful information about his popover.</div>
          </el-popover>

          <el-popover
              placement="bottom"
              popper-class="popover"
              ref="popover4"
              trigger="hover"
              width="200">
            <h3 class="popover-header">Popover On Bottom</h3>
            <div class="popover-body">Here will be some very useful information about his popover.</div>
          </el-popover>

          <n-button type="default" v-popover:popover1>
            On left
          </n-button>
          <n-button type="default" v-popover:popover2>
            On top
          </n-button>
          <n-button type="default" v-popover:popover3>
            On right
          </n-button>
          <n-button type="default" v-popover:popover4>
            On bottom
          </n-button>
        </div>
        <br />
        <br />
        <div class="col-md-6">
          <h4>Datetimepicker</h4>
          <div class="row">
            <div class="col-md-6">
              <div class="datepicker-container">
                <fg-input>
                  <el-date-picker
                      placeholder="Date Time Picker"
                      popper-class="date-picker date-picker-primary"
                      type="datetime"
                      v-model="pickers.dateTimePicker">
                  </el-date-picker>
                </fg-input>
                <fg-input>
                  <el-date-picker
                      placeholder="Date Picker"
                      type="date"
                      v-model="pickers.datePicker">
                  </el-date-picker>
                </fg-input>
                <fg-input>
                  <el-time-select
                      placeholder="Time Picker"
                      v-model="pickers.timePicker">
                  </el-time-select>
                </fg-input>
              </div>
            </div>
          </div>
          <!--                 collapse -->
          <div id="collapse">
            <div class="title">
              <h4>Collapse</h4>
            </div>
            <div class="row">
              <div class="col-md-12">
                <collapse :active-index="0">
                  <collapse-item title="Collapsible Group Item #1">
                    <div>
                      Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry
                      richardson ad squid. 3 wolf
                      moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa
                      nesciunt laborum eiusmod.
                      Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin
                      coffee nulla assumenda
                      shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson
                      cred nesciunt sapiente ea
                      proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer
                      farm-to-table, raw denim
                      aesthetic synth nesciunt you probably haven't heard of them accusamus labore
                      sustainable VHS.
                    </div>
                  </collapse-item>

                  <collapse-item title="Collapsible Group Item #2">
                    <div>
                      Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry
                      richardson ad squid. 3 wolf
                      moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa
                      nesciunt laborum eiusmod.
                      Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin
                      coffee nulla assumenda
                      shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson
                      cred nesciunt sapiente ea
                      proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer
                      farm-to-table, raw denim
                      aesthetic synth nesciunt you probably haven't heard of them accusamus labore
                      sustainable VHS.
                    </div>
                  </collapse-item>

                  <collapse-item title="Collapsible Group Item #3">
                    <div>
                      Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry
                      richardson ad squid. 3 wolf
                      moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa
                      nesciunt laborum eiusmod.
                      Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin
                      coffee nulla assumenda
                      shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson
                      cred nesciunt sapiente ea
                      proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer
                      farm-to-table, raw denim
                      aesthetic synth nesciunt you probably haven't heard of them accusamus labore
                      sustainable VHS.
                    </div>
                  </collapse-item>
                </collapse>
              </div>
            </div>
          </div>
          <!--                 end collapse -->
        </div>
        <div class="col-md-6 tooltip-buttons">
          <h4>Tooltips</h4>
          <el-tooltip class="item" content="Tooltip on the left" placement="left">
            <n-button class="btn btn-default btn-tooltip">On left</n-button>
          </el-tooltip>
          <el-tooltip class="item" content="Tooltip on top" placement="top">
            <n-button class="btn btn-default btn-tooltip">On top</n-button>
          </el-tooltip>
          <el-tooltip class="item" content="Tooltip on bottom" placement="bottom">
            <n-button class="btn btn-default btn-tooltip">On bottom</n-button>
          </el-tooltip>
          <el-tooltip class="item" content="Tooltip on bottom" placement="right">
            <n-button class="btn btn-default btn-tooltip">On right</n-button>
          </el-tooltip>
          <div class="clearfix"></div>
          <br>
          <br>
        </div>
      </div>
    </div>
    <!-- Classic Modal -->
    <modal :show.sync="modals.classic" headerClasses="justify-content-center">
      <h4 class="title title-up" slot="header">Modal title</h4>
      <p>Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live
        the blind texts. Separated they live in Bookmarksgrove right at the coast of the Semantics, a large
        language ocean. A small river named Duden flows by their place and supplies it with the necessary
        regelialia. It is a paradisematic country, in which roasted parts of sentences fly into your
        mouth.</p>
      <template slot="footer">
        <n-button>Nice Button</n-button>
        <n-button @click.native="modals.classic = false" type="danger">Close</n-button>
      </template>
    </modal>

    <!-- notice modal -->
    <modal :show.sync="modals.notice"
           footerClasses="justify-content-center"
           type="notice">
      <h5 class="modal-title" slot="header">How Do You Become an Affiliate?</h5>
      <template>
        <div class="instruction">
          <div class="row">
            <div class="col-md-8">
              <strong>1. Register</strong>
              <p class="description">The first step is to create an account at <a
                  href="https:///www.creative-tim.com/">Creative Tim</a>. You can choose a social
                network or
                go for the classic version, whatever works best for you.</p>
            </div>
            <div class="col-md-4">
              <div class="picture">
                <img alt="Thumbnail Image" class="rounded img-raised" v-lazy="'img/pricing1.jpg'">
              </div>
            </div>
          </div>
        </div>
        <div class="instruction">
          <div class="row">
            <div class="col-md-8">
              <strong>2. Apply</strong>
              <p class="description">The first step is to create an account at <a
                  href="https:///www.creative-tim.com/">Creative Tim</a>. You can choose a social
                network or
                go for the classic version, whatever works best for you.</p>
            </div>
            <div class="col-md-4">
              <div class="picture">
                <img alt="Thumbnail Image" class="rounded img-raised" v-lazy="'img/project9.jpg'">
              </div>
            </div>
          </div>
        </div>
        <p>If you have more questions, don't hesitate to contact us or send us a tweet @creativetim. We're
          here to help!</p>
      </template>
      <div class="justify-content-center" slot="footer">
        <n-button @click.native="modals.notice = false" round type="info">Sounds good!</n-button>
      </div>
    </modal>

    <!-- small modal -->
    <modal :show-close="false"
           :show.sync="modals.mini"
           class="modal-primary"
           headerClasses="justify-content-center"
           type="mini">
      <div class="modal-profile" slot="header">
        <i class="now-ui-icons users_circle-08"></i>
      </div>
      <p>Always have an access to your profile</p>
      <template slot="footer">
        <n-button link type="neutral">Back</n-button>
        <n-button @click.native="modals.mini = false" link type="neutral">Close</n-button>
      </template>
    </modal>
    <modal :show.sync="modals.login"
           class="modal-primary"
           modal-classes="modal-login">
      <div class="card card-plain card-login" data-background-color="" slot="base-content">
        <div class="modal-header justify-content-center">
          <button aria-hidden="true" class="close" data-dismiss="modal" type="button">
            <i class="now-ui-icons ui-1_simple-remove"></i>
          </button>
          <div class="header header-primary text-center">
            <div class="logo-container">
              <img alt="" v-lazy="'img/now-logo.png'">
            </div>
          </div>
        </div>
        <div class="modal-body">
          <form action="" class="form" method="">
            <div class="card-body">
              <fg-input addon-left-icon="now-ui-icons users_circle-08"
                        class="no-border input-lg"
                        placeholder="First Name...">
              </fg-input>

              <fg-input addon-left-icon="now-ui-icons ui-1_lock-circle-open"
                        class="no-border input-lg"
                        placeholder="Password..."
                        type="password">
              </fg-input>
            </div>
          </form>
        </div>
        <div class="modal-footer text-center">
          <a class="btn btn-neutral btn-round btn-lg btn-block" href="#pablo">Get Started</a>
        </div>
      </div>
    </modal>
  </div>
</template>
<script>
  import { Button, Card, Collapse, CollapseItem, FormGroupInput, Modal } from '@/components';
  import { DatePicker, Popover, TimeSelect, Tooltip } from 'element-ui/types';

  export default {
    components: {
      Card,
      Modal,
      CollapseItem,
      Collapse,
      [Button.name]: Button,
      [Popover.name]: Popover,
      [Tooltip.name]: Tooltip,
      [DatePicker.name]: DatePicker,
      [FormGroupInput.name]: FormGroupInput,
      [TimeSelect.name]: TimeSelect
    },
    data () {
      return {
        modals: {
          classic: false,
          notice: false,
          mini: false,
          login: false
        },
        pickers: {
          dateTimePicker: '',
          datePicker: '',
          timePicker: ''
        }
      };
    }
  };
</script>
<style lang="scss">
  #javascriptComponents {
    .modal-buttons,
    .popover-buttons,
    .tooltip-buttons {
      .btn + .btn {
        margin-left: 3px;
      }
    }
  }
</style>
