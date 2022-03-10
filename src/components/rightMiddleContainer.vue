<template>
  <v-container>
    <v-row>
      <v-container white mt-4>
        <h4 class="mb-4">Batches: 1</h4>
        <span class="mdi mdi-chevron-down Down"></span>
      <!-- <v-icon class="icon" red right> mdi-chevron-down </v-icon> -->
        <v-simple-table>
          <template v-slot:default>
            <thead>
              <tr>
                <th class="text-right borderLeft">
                  <span class="mdi mdi-checkbox-blank-outline"></span>
                </th>
                <th class="text-left header"><h4> Batch</h4></th>
                <th class="text-left">Batch ID</th>
                <th class="text-left date" colspan="">Date</th>
                <th></th>
                <th></th>
                <th class="text-left">Saurce</th>
                <th class="text-left">Name</th>
                <th class="text-left borderRight">Raw Count</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td class="borderLeft"><span class="mdi mdi-checkbox-blank-outline"></span></td>
                <td>1</td>
                <td class="abc">409449</td>
                <td colspan="3">Feb 9, 2021</td>
                <td><span class="mdi mdi-newspaper"></span></td>
                <td>postgreSQL</td>
                <td class="borderRight">599</td>
              </tr>
            </tbody>
          </template>
        </v-simple-table>
        <div class="mt-4">
            <p><b><a href="default.asp" target="_blank">Add Batch Info to Dataset</a></b></p>
        </div>
        <!-- <span
          ><p>
            <b
              ><a href="default.asp" success darken-2 class="teg" target="_blank"
                >Add Batch Info to Dataset
              </a></b
            >
          </p></span
        > -->
      </v-container>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>

<style scoped>
.botomButton {
  margin-left: 320px;
}
.borderLeft{
  border-left: 1px solid rgb(197, 194, 194);
  border-radius: 2px;
}
.borderRight{
  border-right: 1px solid rgb(197, 194, 194);
  border-radius: 2px;
}
a:link {
  color: green;
}
th, td {
  border-bottom: 1px solid rgb(197, 194, 194);
  border-top: 1px solid rgb(197, 194, 194);
}
.date{ width: 70%; 
}
th.Date {
  width: 20%; /* Not necessary, since only 70% width remains */
}
.Down{
  float: right;
  margin-top: -40px;
}
ul{
  list-style-type: none;
}
li {
  float: right;
  margin-top: -25px;
}
.fontWeight{
  font-weight: 900;
}
.header{
  font-size: 14px;
}
.abc{
  font-size: 20px;
}
</style>