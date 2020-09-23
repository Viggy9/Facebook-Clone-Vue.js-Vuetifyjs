<template>
    <v-container grid-list-md>
        <v-layout wrap>
            <v-flex xs12 sm8>
                <v-layout wrap column>
                    <v-flex xs12>
                        <v-card rounded outlined>
                            <v-card-title>
                                <v-layout>
                                    <v-btn text class=" font-weight-bold text-none">Make Post</v-btn>
                                    <v-btn text class=" text-none">Live Video</v-btn>
                                    <v-btn text class=" text-none">List</v-btn>
                                </v-layout>
                            </v-card-title>
                            <div class="px-3">
                                <v-layout>
                                    <v-flex xs12>
                                        <v-text-field class=" no-top-padding" background-color="grey lighten-3" height="44px" rounded placeholder="What's on your mind, Vignesh?">
                                    </v-text-field>
                                    </v-flex>
                                </v-layout>
                            </div>
                        </v-card>
                    </v-flex>
                    <v-flex d-inline-flex xs6>
                        <Agash/>
                        
                    </v-flex>
                    <v-flex xs12>
                        <Rahul/>
                        
                    </v-flex>
                </v-layout>
            </v-flex>
            <v-flex xs12 sm4>
                <v-layout wrap column>
                    <v-flex xs12>
                        <Vishal/>
                    </v-flex>
                    <v-flex xs12>
                        <Gokul/>
                    </v-flex>
                </v-layout>
            </v-flex>
        </v-layout>
    </v-container>
</template>

<script>
import Agash from './Feed/Agash'
import Gokul from './Feed/Gokul'
import Rahul from './Feed/Rahul'
import Vishal from './Feed/Vishal'
export default {
    components: {
        Agash,
        Gokul,
        Rahul,
        Vishal
    }
}
</script>

<style>
@import url("//maxcdn.bootstrapcdn.com/font-awesome/4.1.0/css/font-awesome.min.css");
.search { position: relative; }
.search input { text-indent: 30px;}
.search .fa-search { 
  position: absolute;
  top: 24px;
  left: 7px;
  font-size: 15px;
}
.no-top-padding.v-text-field{
    padding-top: 0!important
}

.v-text-field .v-input__append-inner{
    padding-top: 5px;
}


</style>
