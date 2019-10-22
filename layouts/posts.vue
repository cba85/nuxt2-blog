<template>
  <div class="container">
    <div class="row">
      <div class="col-sm-8">
         <nuxt />
      </div>
      <div class="col-sm-4">
            <v-select v-model="selected" placeholder="Select a category" :options="['foo','bar']"></v-select>
      </div>
    </div>
  </div>
</template>
