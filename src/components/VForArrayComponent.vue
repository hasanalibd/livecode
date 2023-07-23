<script setup>
const items = [

  {
    id: 1,
    title: "Item 1",
    description: "Description for Item 1"
  },

  {
    id: 2,
    title: "Item 2",
    description: "Description for Item 2"
  },

  {
    id: 3,
    title: "Item 3",
    description: "Description for Item 3"
  },

  {
    id: 4,
    title: "Item 4",
    description: "Description for Item 4"
  },

  {
    id: 5,
    title: "Item 5",
    description: "Description for Item 5"
  },

  {
    id: 6,
    title: "Item 6",
    description: "Description for Item 6"
  }

];
</script>

<template>
  <div>
    <ul class="unorderlist">
      <li v-for="item in items" :key="item.id">
        <h2>{{ item.title }}</h2>
        <p>{{ item.description }}</p>
      </li>
    </ul>
  </div>
</template>

<style scoped>
.unorderlist{
  list-style-type: none;
}
li{
  background-color: rgb(233, 233, 233);
  padding: 10px 50px;
  margin-top: 10px;
}
</style>
