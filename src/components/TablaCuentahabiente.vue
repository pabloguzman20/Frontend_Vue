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
        { text: "nombre", value: "nom" },
        { text: "telefono", value: "tel" },
        { text: "Created At", value: "fechaCreacion" },
        { text: "Updated At", value: "fechaActualizacion" }
      ],
      desserts: [
        {
          name: "1",
          nom: "Pablo Guzman",
          tel: 6863243241,
          fechaCreacion: "2020-11-8",
          fechaActualizacion: "2020-11-28"
        },
        {
          name: "2",
          nom: "Juan Lopez",
          tel: 6863854025,
          fechaCreacion: "2020-11-12",
          fechaActualizacion: "2020-11-22"
        }
      ]
    };
  }
};
</script>
