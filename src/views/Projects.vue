<template>
  <b-container class="hours-log-page">
    <b-row>
      <b-col sm="8" offset-sm="2">
        <b-row class='mt-5'>
          <b-col>
            <h1>Projects</h1>
          </b-col>
          <b-col>
            <b-btn variant="outline-primary">
              + Add New Project
            </b-btn>
          </b-col>
        </b-row>
        <b-row>
          <b-col>
            <v-select 
            :options="[{label: 'Canada', code: 'ca'}]">
            </v-select>
          </b-col>
        </b-row>
      </b-col>
    </b-row>
  </b-container>
</template>