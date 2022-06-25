<template>
<table class="table table-striped table-bordered">
      <thead>
        <tr>
          <th>Nama</th>
          <th>Stok</th>
          <th>Status</th>
        </tr>
      </thead>
      <tbody>
        <tr  v-for="item in items" :key="item">
          <!-- <th scope="row">1</th> -->
          <td>{{ item.nama }}</td>
          <td>{{ item.stok }}</td>
          <td v-if="item.stok == 0">Tidak Tersedia</td>
          <td v-else>Tersedia</td>
        </tr>
        <!-- <td>
          <tr v-for="item in items" :key="item">{{ item.nama }}</tr>
        </td>
        <td>
          <tr v-for="item in items" :key="item">{{ item.stok }}</tr>
        </td>
        <td>
          <tr v-for="item in items" :key="item">{{ item.stok >= 0 ? "Tidak Tersedia" : "Tersedia" }}</tr>
        </td> -->
      </tbody>


    </table>
</template>

<script>
import file from "@/static/product.js"
export default {
  data() {
    return {
      name: 'App',
      items: file.Products,
    }
  }
}
</script>

<style>

</style>