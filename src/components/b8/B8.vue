<template>
  <div>
    <h2>B8</h2>
    <v-card>
    <v-tabs
      v-model="tab"
      bg-color="primary"
    >
      <v-tab value="one">Trang Chu</v-tab>
      <v-tab value="two">Gioi Thieu</v-tab>
      <v-tab value="three">Lien He</v-tab>
    </v-tabs>

    <v-card-text>
      <v-tabs-window v-model="tab">
        <v-tabs-window-item value="one">
          Trang Chu
        </v-tabs-window-item>

        <v-tabs-window-item value="two">
          Gioi Thieu
        </v-tabs-window-item>

        <v-tabs-window-item value="three">
          Lien He
        </v-tabs-window-item>
      </v-tabs-window>
    </v-card-text>
  </v-card>
  </div>
</template>

<script>
export default {
    data: () => ({
      tab: null,
    }),
}
</script>

<style>

</style>