<template>
  <v-toolbar class="brown lighten-3" light>
    <v-toolbar-side-icon light></v-toolbar-side-icon>
    <v-toolbar-title>Toolbar</v-toolbar-title>
    <v-toolbar-items>
      <v-menu origin="right center"
      transition="v-scale-transition"
      left >
        <v-btn light icon slot="activator">
          <v-icon>more_vert</v-icon>
        </v-btn>
        <v-list>
          <v-list-item>
            <v-list-tile router action="link" href="/view_past_month_timesheets">
 <v-list-tile-title>Previous month timesheet</v-list-tile-title>
            </v-list-tile>
            <v-list-tile router action="link" href="/view_current_month_timesheet">
   
  <v-list-tile-title>Current month timesheet</v-list-tile-title>

            </v-list-tile>
            <v-list-tile router action="link" href="/generate_this_month_timesheet">
  <v-list-tile-title>Generate this month timesheet</v-list-tile-title>
            </v-list-tile>


            <v-list-tile>
             <v-list-tile router action="link" href="/Login">
              <v-list-tile-title>Log Out</v-list-tile-title>
            </v-list-tile>
          </v-list-item>
        </v-list>
      </v-menu>
    </v-toolbar-items>
  </v-toolbar>
</template>
<script>
export default {
  name: 'Top'
}
</script>

<style scoped>
  header {
    border-bottom: 1px solid #42b983;
    margin-bottom: 30px;
    height: 10vh;
  }
</style>