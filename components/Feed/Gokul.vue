<template>
  <v-card rounded outlined>
    <v-layout wrap>
      <v-flex v-for="n in 2" :key="n" xs6>
        <v-card flat tile>
          <v-img
            :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
            :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
            aspect-ratio="1"
            class="grey lighten-2"
          ></v-img>
        </v-card>
      </v-flex>
    </v-layout>
           <v-card-title>
                <div class=" font-weight-bold" style="font-size: 17px">Join PhotoApp for Photography Lessons</div>
            </v-card-title>
    <v-card-text>
      <div class="questrial body1 mb-4">{{lorem}}</div>
    </v-card-text>
  </v-card>
</template>

<script>
import Emojis from "../Emoji/Emojis";
export default {
  components: {
    Emojis
  },
  data() {
    return {
      lorem: `Lorem ipsum dolor sit amet, mel at clita quando. Te sit oratio vituperatoribus, nam ad ipsum posidonium mediocritatem, explicari dissentiunt cu mea. Repudiare disputationi vim in, mollis iriure nec cu, alienum argumentum ius ad. Pri eu justo aeque torquatos.`
    };
  }
};
</script>

<style>
</style>
