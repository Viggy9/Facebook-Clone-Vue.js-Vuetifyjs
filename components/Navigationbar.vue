<template>
    <v-navigation-drawer width="300px" color="#e9ebee" floating clipped app permanent>
        <v-container>
            <v-card color="#e9ebee" rounded outlined>
                 <v-list-item class="pt-2">
                    <v-list-item-avatar>
                         <v-icon left>mdi-face-profile</v-icon>
                    </v-list-item-avatar>
                    <v-list-item-content>
                        <v-list-item-title class="subtitle">Vignesh</v-list-item-title>
                    </v-list-item-content>
                </v-list-item>
                
                <v-list>
                    
                    <v-list-item-group v-model="item" active-class="active-list-item">
                         <v-list-item :key="index" v-for="(item,index) in items" dense style="height:20px" >
                            <v-list-item-action>
                                <v-icon>{{item.icon}}</v-icon>
                            </v-list-item-action>
                            <v-list-item-content>
                                
                                <v-list-item-title class="body1">{{item.text}}</v-list-item-title>
                            </v-list-item-content>
                        </v-list-item>
                    </v-list-item-group>
                </v-list>
            </v-card>
        </v-container>
    </v-navigation-drawer>
</template>

<script>
export default {
    data(){
        return {
            item: 1,
            items: [
                {text: 'News Feed', icon: 'mdi-note-text'},
                {text: 'Messenger', icon: 'mdi-comment-multiple-outline'},
                {text: 'Watch', icon: 'mdi-video'},

            ]
        }
    }
}
</script>

<style>
.active-list-item .v-list-item--dense .v-list-item__title, .v-list-item--dense .v-list-item__subtitle, .v-list--dense .v-list-item .v-list-item__title, .v-list--dense .v-list-item .v-list-item__subtitle {
    font-family: 'Questrial';
    font-weight: 'bold';
}
</style>
