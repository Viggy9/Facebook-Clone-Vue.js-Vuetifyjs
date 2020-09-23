<template>
    <v-card rounded outlined>
        <div>
            <v-list-item>
                <v-list-item-content class="mt-2">
                    <v-list-item-title class="questrial subtitle text-center">Ads</v-list-item-title>
                </v-list-item-content>
            </v-list-item>
        </div>
        <!-- <v-container grid-list-xs fluid style="padding:10px"> -->
            <v-layout wrap>
                <v-flex xs12>
                    <v-card flat tile>
                        <v-img
                        :src="`https://picsum.photos/500/300?image=${12 * 5 + 10}`"
                        :lazy-src="`https://picsum.photos/10/6?image=${12 * 5 + 10}`"
                        aspect-ratio="2"
                        class="grey lighten-2"
                        gradient="to top right, rgba(0,0,0,.2), rgba(0,0,0,.2)"
                        >
                            <v-layout
                            fill-height
                            align-center
                            justify-center
                            ma-0
                            >
                        
                                    
                            </v-layout>
                        </v-img>
                    </v-card>
                </v-flex>
                
            </v-layout>
            <v-card-title>
                <div class="questrial font-weight-bold" style="font-size: 17px">Join IndiaRun for Outdoor Excerises</div>
            </v-card-title>
            <v-card-text>
            <div class="questrial body1 mb-4">{{lorem}}</div>
            <v-layout class="py-4">
            </v-layout>
            <v-divider></v-divider>
            
        </v-card-text>
        <!-- </v-container> -->
    </v-card>
</template>

<script>
import Emojis from '../Emoji/Emojis'
export default {
    components:{
        Emojis,
    },
    data(){
        return {
            lorem: `Lorem ipsum dolor sit amet, mel at clita quando. Te sit oratio vituperatoribus, nam ad ipsum posidonium mediocritatem, explicari dissentiunt cu mea. Repudiare disputationi vim in, mollis iriure nec cu, alienum argumentum ius ad. Pri eu justo aeque torquatos.`,
        }
    }
}
</script>

<style>
.v-menu__content{
    border-radius: 25px
}
</style>
