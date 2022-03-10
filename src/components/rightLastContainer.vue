<template>
<v-container white class="mt-4">
    <div class="mt-4">
      <h3>Properties</h3>
      <p><b>Name:</b> customer weekly</p>
      <p>created on January 21, 2021 14:42 by Nuno Mura </p>
      <v-divider class="mt-2 mb-2"></v-divider>
      <div>
        <p1><b>Rows:</b> 699 <b>Columns:</b> 10</p1><br>
        <p1><b>Size</b> 160.00 KB</p1>
      <v-divider class="mt-2 mb-2"></v-divider>
        <v-container fluid>
        <v-row no-gutters>
          <v-col cols="6">
      <h4>DATA RETRIEVAl SCHEDULE </h4>
        <p1><b>Every week on Monday</b></p1><br>
        <p1><b>Range:</b>Start January 25, 2021 14:42 </p1><br>
        <p1><b>Datapull Status:</b> Successfull </p1>
          </v-col>
          <v-col cols="2">
          </v-col>
          <v-col cols="4">
            <p><b><a href="default.asp" target="_blank">Edit conections</a></b></p>
            <p class="anchorTeg"><b><a href="default.asp" target="_blank">Retreive latest data</a></b></p>
          </v-col>  
        </v-row>
        </v-container>      
      </div>
    </div>
</v-container>
</template>

<script>
export default {

}
</script>

<style>
.LastComponent{
    background: white;
}
.anchorTeg{
  margin-top: -15px;
}

a:link {
  color: green !important;
}
a:hover {
  color: black;
}
</style>