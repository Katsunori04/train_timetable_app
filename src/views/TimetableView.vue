<template>
  <div class="about">
    <h1>timetable page</h1>
    <TimeCard :stations = "stations"></TimeCard>
    <TimeBoard></TimeBoard>
  </div>
</template>

<script>
import TimeCard from "../components/TimeCard.vue"
import TimeBoard from "../components/TimeBoard.vue"

export default {
  name: "App",
  components: {
    TimeCard,
    TimeBoard,
  },

  data: () => ({
    stations: {
      name: '駒川中野',
      name_en: 'Komagawa Nakano',
      next_time: '10:00',
      next: '',
      prev: '',
    },
  }),
}
</script>

<style>

</style>