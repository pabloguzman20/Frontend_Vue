<template>
  <v-data-table
    :headers="headers"
    :items="desserts"
    :items-per-page="5"
    class="elevation-1"
  ></v-data-table>
</template>

<script>
export default {
  data() {
    return {
      headers: [
        {
          text: "id",
          align: "start",
          sortable: false,
          value: "name"
        },
        { text: "Saldo", value: "saldo" },
        { text: "Created At", value: "fechaCreacion" },
        { text: "Updated At", value: "fechaActualizacion" }
      ],
      desserts: [
        {
          name: "1",
          saldo: 200000,
          fechaCreacion: "2020-11-8",
          fechaActualizacion: "2020-11-28"
        },
        {
          name: "2",
          saldo: 50000,
          fechaCreacion: "2020-11-12",
          fechaActualizacion: "2020-11-22"
        }
      ]
    };
  }
};
</script>
