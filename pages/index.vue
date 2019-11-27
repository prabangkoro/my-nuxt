<template>
  <v-container fluid class="pa-0"
    style="height: 100%;"
  >
    <v-row
      align="center"
      justify="center"
      style="height: 100%;"
    >
      <box>
        {{ prayers[selected] }}
      </box>
    </v-row>
    <div class="d-flex justify-space-between mt-n10">
      <div>
        <v-btn
          v-show="selected !== 0"
          color="rgba(256, 256, 256, 0.75)"
          text
          @click="selected = selected - 1"
        >
          Prev
        </v-btn>
      </div>
      <div>
        <v-btn
          v-show="selected !== (prayers.length - 1)"
          color="rgba(256, 256, 256, 0.75)"
          text
          @click="selected = selected + 1"
        >
          Next
        </v-btn>
      </div>
    </div>
  </v-container>
</template>

<script>
import Box from '~/components/Box'
export default {
  components: {
    Box
  },
  data () {
    return {
      prayers: [
        'Untuk Noor',
        'ku panjatkan doa,',
        'agar senantiasa diberi ruangan untuk berkembang dan belajar,',
        'belajar dari naik turun nya hidup,',
        'hidup memang unexpected, tapi kamu bisa menikmati setiap detiknya,',
        'hidup terakselerasi year-by-year,',
        'terus explore hal baru di luar zona nyaman,',
        'paham mana buruk mana benar, mengambil keputusan dengan bijak.',
        'Keep smile, you deserved to be happy :)',
        'Somebody loves you',
        'Keep inspires other',
        'from your friend Babang'
      ],
      selected: 0
    }
  }
}
</script>
