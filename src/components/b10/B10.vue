<template>
<div>
  <h2>B10</h2>
  <v-container>
    <v-card>
      <v-card-title>Item</v-card-title>
      <table class="custom-table">
        <thead>
          <tr>
            <th>Name</th>
            <th>Project Name</th>
            <th>Post</th>
            <th>Status</th>
            <th>Budget</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="(item, index) in items" :key="index">
            <td>{{ item.name }}</td>
            <td>{{ item.projectName }}</td>
            <td>{{ item.post }}</td>
            <td>
              <v-chip
                :color="getStatusColor(item.status)"
                text-color="white"
                small
              >
                {{ item.status }}
              </v-chip>
            </td>
            <td>{{ item.budget }}</td>
          </tr>
        </tbody>
      </table>
    </v-card>
  </v-container>
</div>
  
</template>

<script setup>
const items = [
  { name: 'Sunil Joshi', projectName: 'Elite Admin', post: 'Web Designer', status: 'Active', budget: '$3.9' },
  { name: 'Andrew McDownland', projectName: 'Real Homes WP Theme', post: 'Project Manager', status: 'Pending', budget: '$24.5k' },
  { name: 'Christopher Jamil', projectName: 'MedicalPro WP Theme', post: 'Project Manager', status: 'Completed', budget: '$12.8k' },
  { name: 'Nirav Joshi', projectName: 'Hosting Press HTML', post: 'Frontend Engineer', status: 'Active', budget: '$2.4k' },
  { name: 'Micheal Doe', projectName: 'Helping Hands WP Theme', post: 'Content Writer', status: 'Cancel', budget: '$9.3k' },
];

const getStatusColor = (status) => {
  switch (status) {
    case 'Active':
      return 'green lighten-2';
    case 'Pending':
      return 'orange lighten-2';
    case 'Completed':
      return 'blue lighten-2';
    case 'Cancel':
      return 'red lighten-2';
    default:
      return 'grey lighten-2';
  }
};
</script>

<style scoped>
.custom-table {
  width: 100%;
  border-collapse: collapse;
}

.custom-table th,
.custom-table td {
  padding: 10px;
  text-align: left;
  border-bottom: 1px solid #ddd;
}

.custom-table th {
  background-color: #f5f5f5;
}

.v-card {
  padding: 20px;
}
</style>
