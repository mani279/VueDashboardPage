<template>
  <div class="q-pa-md">
    <div class="row q-col-gutter-md">
      <div class="col-xl-4 col-lg-4 col-md-4 col-sm-12 col-xs-12">
        <q-card class="my-card col bg-white text-secondary">
          <q-card-section class="row items-center">
            <div class="col-xl-1 col-lg-1 col-md-2 col-sm-1 col-xs-3">
              <QAvatar
                color="secondary"
                text-color="white"
                icon="bar_chart"
              />
            </div>
            <div class="col-xl-10 col-lg-10 col-md-8 col-sm-10 col-xs-7">
              <div class="row items-center">
                <div class="q-pl-md text-text-caption">Statistics</div>
              </div>
              <div class="row items-center">
                <div class="q-pl-md text-subtitle2">5439</div>
              </div>
            </div>
            <div class="col">
              <QAvatar text-color="secondary" icon="arrow_right_alt" />
            </div>
          </q-card-section>
        </q-card>
      </div>
      <div class="col-xl-4 col-lg-4 col-md-4 col-sm-12 col-xs-12">
        <q-card class="my-card col bg-white text-secondary">
          <q-card-section class="row items-center">
            <div class="col-xl-1 col-lg-1 col-md-2 col-sm-1 col-xs-3">
              <QAvatar
                color="secondary"
                text-color="white"
                icon="people"
              />
            </div>
            <div class="col-xl-10 col-lg-10 col-md-8 col-sm-10 col-xs-7">
              <div class="row items-center">
                <div class="q-pl-md text-text-caption">Users</div>
              </div>
              <div class="row items-center">
                <div class="q-pl-md text-subtitle2">2k</div>
              </div>
            </div>
            <div class="col">
              <QAvatar text-color="secondary" icon="arrow_right_alt" />
            </div>
          </q-card-section>
        </q-card>
      </div>
      <div class="col-xl-4 col-lg-4 col-md-4 col-sm-12 col-xs-12">
        <q-card class="my-card col bg-white text-secondary">
          <q-card-section class="row items-center">
            <div class="col-xl-1 col-lg-1 col-md-2 col-sm-1 col-xs-3">
              <QAvatar
                color="secondary"
                text-color="white"
                icon="download"
              />
            </div>
            <div class="col-xl-10 col-lg-10 col-md-8 col-sm-10 col-xs-7">
              <div class="row items-center">
                <div class="q-pl-md text-text-caption">Sales</div>
              </div>
              <div class="row items-center">
                <div class="q-pl-md text-subtitle2">2.2k</div>
              </div>
            </div>
            <div class="col">
              <QAvatar text-color="secondary" icon="arrow_right_alt" />
            </div>
          </q-card-section>
        </q-card>
      </div>
    </div>

    <div class="row q-col-gutter-md q-pt-md">
      <div class="col-xl-4 col-lg-4 col-md-4 col-sm-12 col-xs-12">
        <q-card class="my-card col bg-white text-secondary">
          <q-card-section class="row items-center">
            <div class="col-xl-1 col-lg-1 col-md-2 col-sm-1 col-xs-3">
              <QAvatar
                color="secondary"
                text-color="white"
                icon="inventory_2"
              />
            </div>
            <div class="col-xl-10 col-lg-10 col-md-8 col-sm-10 col-xs-7">
              <div class="row items-center">
                <div class="q-pl-md text-text-caption">New Products</div>
              </div>
              <div class="row items-center">
                <div class="q-pl-md text-subtitle2">15</div>
              </div>
            </div>
            <div class="col">
              <QAvatar text-color="secondary" icon="arrow_right_alt" />
            </div>
          </q-card-section>
        </q-card>
      </div>
      <div class="col-xl-4 col-lg-4 col-md-4 col-sm-12 col-xs-12">
        <q-card class="my-card col bg-white text-secondary">
          <q-card-section class="row items-center">
            <div class="col-xl-1 col-lg-1 col-md-2 col-sm-1 col-xs-3">
              <QAvatar
                color="secondary"
                text-color="white"
                icon="local_offer"
              />
            </div>
            <div class="col-xl-10 col-lg-10 col-md-8 col-sm-10 col-xs-7">
              <div class="row items-center">
                <div class="q-pl-md text-text-caption">Discount</div>
              </div>
              <div class="row items-center">
                <div class="q-pl-md text-subtitle2">15%</div>
              </div>
            </div>
            <div class="col">
              <QAvatar text-color="secondary" icon="arrow_right_alt" />
            </div>
          </q-card-section>
        </q-card>
      </div>
      <div class="col-xl-4 col-lg-4 col-md-4 col-sm-12 col-xs-12">
        <q-card class="my-card col bg-white text-secondary">
          <q-card-section class="row items-center">
            <div class="col-xl-1 col-lg-1 col-md-2 col-sm-1 col-xs-3">
              <QAvatar
                color="secondary"
                text-color="white"
                icon="trending_up"
              />
            </div>
            <div class="col-xl-10 col-lg-10 col-md-8 col-sm-10 col-xs-7">
              <div class="row items-center">
                <div class="q-pl-md text-text-caption">Growth</div>
              </div>
              <div class="row items-center">
                <div class="q-pl-md text-subtitle2">90%</div>
              </div>
            </div>
            <div class="col">
              <QAvatar text-color="secondary" icon="arrow_right_alt" />
            </div>
          </q-card-section>
        </q-card>
      </div>
    </div>
  </div>
</template>
<script>
import { QAvatar } from "quasar";
export default {
  name: "StockCards",
  components: {
    QAvatar: QAvatar,
  },
  data() {
    return {};
  },
};
</script>
