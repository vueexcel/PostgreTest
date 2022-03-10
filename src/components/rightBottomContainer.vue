<template>
  <v-container white mt-4>
    <h3 class="mb-3">Preview</h3>
    <span class="mdi mdi-chevron-down Down"></span>
    <template>
      <v-col class="d-flex Select" cols="8">
        <v-select :items="items" label="View Steps" dense outlined></v-select>
        <v-select
          class="ml-4"
          :items="items"
          label="Latest 4 Steps|5"
          dense
          outlined
        ></v-select>
      </v-col>
    </template>
    <v-simple-table class="Table">
      <template v-slot:default>
        <thead>
          <tr class="tr">
            <th class="text-left TH">#</th>
            <th class="text-left TH">customer_id</th>
            <th class="text-left TH">store_id</th>
            <th class="text-left TH">first_name</th>
            <th class="text-left TH">last_name</th>
            <th class="text-left TH">email</th>
            <th class="text-left TH">address_id</th>
            <th class="text-left TH">activeboll</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="item in desserts" :key="item.store_id">
            <td class="TD">{{ item.serialNo }}</td>
            <td class="TD">{{ item.customer_id }}</td>
            <td class="TD">{{ item.store_id }}</td>
            <td class="TD">{{ item.first_name }}</td>
            <td class="TD">{{ item.last_name }}</td>
            <td class="TD">{{ item.email }}</td>
            <td class="TD">{{ item.address_id }}</td>
            <td class="TD">{{ item.activeboll }}</td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      desserts: [
        {
          serialNo: "1",
          customer_id: "524",
          store_id: "1",
          first_name: 159,
          last_name: "ELY",
          email: "jared.ely@sakilgmail",
          address_id: "530",
          activeboll: "t",
        },
        {
          serialNo: "2",
          customer_id: "1",
          store_id: "1",
          first_name: 237,
          last_name: "Smith",
          email: "jared.ely@sakilgmail",
          address_id: "530",
          activeboll: "t",
        },
        {
          serialNo: "3",
          customer_id: "3",
          store_id: "1",
          first_name: 262,
          last_name: "jam",
          email: "jared.ely@sakilgmail",
          address_id: "530",
          activeboll: "t",
        },
        {
          serialNo: "4",
          customer_id: "4",
          store_id: "1",
          first_name: 305,
          last_name: "sum",
          email: "jared.ely@sakilgmail",
          address_id: "530",
          activeboll: "t",
        },
        {
          serialNo: "5",
          customer_id: "5",
          store_id: "1",
          first_name: 518,
          last_name: "jack",
          email: "jared.ely@sakilgmail",
          address_id: "530",
          activeboll: "t",
        },
      ],
    };
  },
};
</script>

<style scoped>
</style>

<style scoped>
table,
th,
td {
  border: 1px solid rgb(197, 194, 194);
}

.TD {
  font-size: 12px !important;
  height: 23px !important;
}
.TH {
  font-weight: 900;
  width: 30px;
}
.rightText {
  font-size: 14px;
}
.Table {
  margin-top: -15px;
}
a:link {
  color: green;
}
.Down {
  float: right;
  margin-top: -40px;
}
.Select {
  margin-left: -10px;
}
</style>