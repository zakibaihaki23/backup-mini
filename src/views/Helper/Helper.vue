<template>
  <div class="helper">
    <h2>HELPER LIST</h2>
    <v-container>
      <v-row no-gutters>
        <v-col md="6">
          <div>
            <v-btn>Registration Helper</v-btn>
          </div>
        </v-col>
        <v-col md="6" offset="6">
          <div class="search">
            <v-text-field
              append-icon="mdi-magnify"
              rounded
              label="Search...."
              solo
              append-outer-icon="mdi-format-align-justify"
            >
            </v-text-field>
          </div>
        </v-col>
      </v-row>
    </v-container>
    <p style="font-size: 20px">Filter</p>
    <v-col md="12">
      <v-divider style="margin-right: 40px"></v-divider>
    </v-col>
    <v-row>
      <v-col cols="2">
        <v-select
          style="border-radius: 15px"
          outlined
          label="Status"
          solo
        ></v-select>
      </v-col>
      <v-col cols="2">
        <v-select
          style="border-radius: 15px"
          outlined
          label="Warehouse"
          solo
        ></v-select>
      </v-col>
    </v-row>
    <br />
    <v-data-table hide-default-footer> </v-data-table>
    <div class="text-left pt-2">
      <v-pagination></v-pagination>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {}
    },
  }
</script>

<style scoped>
  .helper {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
      Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    padding-left: 80px;
    padding-right: 50px;
  }
  .v-btn:not(.v-btn--round).v-size--default {
    position: absolute;
    width: 178px;
    height: 50px;
    background: #4662d4;
    color: white;
    border-radius: 25px;
    box-sizing: content-box;
    margin-top: 50px;
    text-transform: capitalize;
    cursor: pointer;
  }
  .search {
    padding-left: 100px;
    padding-right: 50px;

    margin-top: 50px;
  }
</style>
