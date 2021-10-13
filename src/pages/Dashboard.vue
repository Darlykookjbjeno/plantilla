<template>
  <div class="content">

    <div class="row">
      <div class="col-12">
        <card type="chart">
          <template slot="header">
            <div class="row">
              <div class="col-sm-6" :class="isRTL ? 'text-right' : 'text-left'">
                <template>
                  <h5 class="card-category">Total Shipments</h5>
                </template>

                <template>
                  <h2 class="card-title">Performance</h2>
                </template>
              </div>
            </div>
          </template>
        </card>
      </div>
    </div>



    <div class="row">
      <div class="col-lg-12 col-md-12">
        <card class="card">
          <h4 slot="header" class="card-title">
            <template> Simple Table </template>
          </h4>
          <div class="table-responsive">
            <user-table></user-table>
          </div>
        </card>
      </div>
    </div>

  </div>
</template>



<script>
import { Card } from "@/components/index";

import LineChart from "@/components/Charts/LineChart";
import BarChart from "@/components/Charts/BarChart";
// import * as chartConfigs from "@/components/Charts/config";
import TaskList from "./Dashboard/TaskList";
import UserTable from "./Dashboard/UserTable";


export default {
  components: {
    Card,
    LineChart,
    BarChart,
    TaskList,
    UserTable,
  },

};
</script>
<style>
</style>
