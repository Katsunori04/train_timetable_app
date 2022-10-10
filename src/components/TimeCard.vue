<template>
  <v-card max-width="344" outlined>
    <v-list-item three-line>
      <v-list-item-content>
        <v-list-item-title class="text-h5 mt-5 mb-1 text-center font-weight-bold">
          
          {{stations.name}}
        </v-list-item-title>
          <p class="text-center mt-3 font-weight-black pa-1 bg-purple-darken-2 ">{{stations.name_en}}</p>
      </v-list-item-content>
      <v-list-item-avatar tile size="80" color="grey"></v-list-item-avatar>
    </v-list-item>
    <v-spacer class="mb-5"></v-spacer>
  </v-card>
</template>

<script>
export default {
  name: 'TimeCard',

  props: {
    stations: {
      default: {
                name: '駒川中野',
                name_en: 'Komagawa Nakano',
                next_time: '10:00',
                next: '',
                prev: '',
      },
    },
  },
  data: () => ({
    //
  }),
}
</script>