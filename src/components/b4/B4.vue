<template>
  <div>
    <h2>B4</h2>
    <div class="">
    <v-menu>
      <template v-slot:activator="{ props }">
        <v-btn
          color="primary"
          v-bind="props"
        >
          Quan tri vien
        </v-btn>
      </template>
      <v-list>
        <v-list-item
          v-for="(item, index) in items"
          :key="index"
          :value="index"
        >
          <v-list-item-title>{{ item.title }}</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-menu>
  </div>
  </div>
</template>

<script>
export default {
    data: () => ({
      items: [
        { title: 'Thong tin ca nhan' },
        { title: 'Doi mat khau' },
        { title: 'Dang xuat' },
      ],
    }),
  }
</script>

<style>

</style>