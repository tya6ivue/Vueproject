<template>
  <div>
    <div v-if="show">
      <table border="1px">
        <tr>
          <th>Id</th>
          <th>Name</th>
          <th>email</th>
        </tr>
        <tr v-for="item in users" :key="item.id">
          <td>{{ item.id }}</td>
          <td>{{ item.name }}</td>
          <td>{{ item.email }}</td>
        </tr>
      </table>
    </div>
    <button v-on:click="btn">buttonn</button>
  </div>
</template>

<script>
export default {
  name: "Home2",
  data() {
    return (
      {
        show: false,
      },
      {
        users: [
          { id: 1, name: "Peter", email: "Peter@gmail.com" },
          { id: 1, name: "Bruce", email: "bruce@gmail.com" },
          { id: 1, name: "Jorge", email: "jorge@gmail.com" },
          { id: 1, name: "Tony", email: "tony@gmail.com" },
          { id: 1, name: "Sam", email: "Sam@gmail.com" },
        ],
      }
    );
  },
  methods: {
    btn() {
      this.show = !this.show;
    },
  },
};
</script>