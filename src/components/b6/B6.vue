<template>
  <div>
    <h2>B6</h2>
    <div class="pa-4">
      <v-btn @click="dialog = true"> Xac Nhan </v-btn>

      <v-dialog v-model="dialog" width="auto">
        <v-card
          max-width="400"
          prepend-icon="mdi-update"
          text="Le Dien Tien co deeptry khong ?"
          title="Xac Nhan"
        >
          <template v-slot:actions>
            <v-btn class="ms-auto" text="Co deeptry " @click="dialog = false"></v-btn>
          </template>
        </v-card>
      </v-dialog>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      dialog: false,
    };
  },
};
</script>

<style></style>
