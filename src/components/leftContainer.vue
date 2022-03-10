<template>
  <v-container class="w-100" fluid>
    <v-row no-gutters>
      <v-col lg="12" class="w-50">
        <v-simple-table>
          <template v-slot:default>
            <thead class="tHead">
              <tr>
                <th class="text-left"></th>
                <th class="text-left">File Name</th>
                <th class="text-left">Cols | Rows</th>
                <th class="text-left">
                  Last modified
                  <span class="mdi mdi-arrow-down-drop-circle-outline"></span>
                </th>
              </tr>
            </thead>
            <tbody>
              <tr v-for="item in desserts" :key="item.fileName">
                <td>
                  <div><img :src="item.avatar" class="img" /></div>
                </td>
                <td>{{ item.fileName }}</td>
                <td>{{ item.ColsRows }}</td>
                <td>{{ item.lastModified }}</td>
              </tr>
            </tbody>
          </template>
        </v-simple-table>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      desserts: [
        {
          avatar: require("../../public/postgresql.svg"),
          fileName: "Customer weekly",
          ColsRows: 159,
          lastModified: "9 minutes ago",
        },
        {
          avatar: require("../../public/postgresql.svg"),
          fileName: "Film actor",
          ColsRows: 237,
          lastModified: "9 minutes ago",
        },
        {
          avatar: require("../../public/postgresql.svg"),
          fileName: "Customer",
          ColsRows: 262,
          lastModified: "9 minutes ago",
        },
        {
          avatar: require("../../public/postgresql.svg"),
          fileName: "Result Dataset",
          ColsRows: 305,
          lastModified: "9 minutes ago",
        },
        {
          avatar: require("../../public/postgresql.svg"),
          fileName: "Result ",
          ColsRows: 518,
          lastModified: "9 minutes ago",
        },
        {
          avatar: "",
          fileName: "view 4",
          ColsRows: 518,
          lastModified: "9 minutes ago",
        },
        {
          avatar: "",
          fileName: "view 3",
          ColsRows: 518,
          lastModified: "9 minutes ago",
        },
        {
          avatar: "",
          fileName: "view 2",
          ColsRows: 518,
          lastModified: "9 minutes ago",
        },
        {
          avatar: "",
          fileName: "view 1",
          ColsRows: 518,
          lastModified: "9 minutes ago",
        },
        {
          avatar: require("../../public/Anonymous_Paper_2_icon.svg"),
          fileName: "Result Dataset",
          ColsRows: 518,
          lastModified: "9 minutes ago",
        },
        {
          avatar: require("../../public/postgresql.svg"),
          fileName: "KitKat",
          ColsRows: 518,
          lastModified: "9 minutes ago",
        },
        {
          avatar: require("../../public/postgresql.svg"),
          fileName: "KitKat",
          ColsRows: 518,
          lastModified: "9 minutes ago",
        },
        {
          avatar: require("../../public/postgresql.svg"),
          fileName: "KitKat",
          ColsRows: 518,
          lastModified: "9 minutes ago",
        },
        {
          avatar: require("../../public/postgresql.svg"),
          fileName: "KitKat",
          ColsRows: 518,
          lastModified: "9 minutes ago",
        },
      ],
    };
  },
};
</script>

<style>
.img {
  height: 15px;
}
.tHead {
  background: #eceff1;
}
</style>