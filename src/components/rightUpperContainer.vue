<template>
  <v-container class="fluid" fluid white>
    <v-col>
      <v-icon class="icon" red right> mdi-close </v-icon>
      <h4  class="upperText">Customer weekly</h4>
      <h5 class="middleText"><b> Last Updated:</b> 9 minutes ago</h5>
      <div class="d-flex mt-4">
        <button small class="Button">Open</button>
        <div class="mt-1">
          <span class="mdi mdi-dots-vertical ml-4 mb-2"></span>
        </div>
        <div class="icon">
          <v-icon class="mt-2" red right> mdi-delete </v-icon>
        </div>
      </div>
    </v-col>
  </v-container>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>

<style>
.Button {
  width: 120px;
  background-color: #2f702e;
  color: white;
  margin-left: -10px;
}
.icon {
  float: right;
  margin-left: 300px;
}
.upperText{
  font-weight: 600;
  font-size: 18px;
  margin-left: -10px;
}
.middleText{
  margin-left: -10px;
  font-weight: 400;
}
</style>