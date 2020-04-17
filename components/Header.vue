<template>
    <div>
    <v-toolbar dense
    height="75px" 
    >
      <v-toolbar-title class="head-logo"><img src="~/assets/Logo.png"></v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
          <div class="menu-item">
                <v-menu open-on-hover bottom offset-y>
                <template v-slot:activator="{ on }">
                    <v-btn
                    text
                    small
                    color="#104388"
                    v-on="on"
                    >
                    How it works
                    <v-icon right dark>mdi-menu-down</v-icon>
                    </v-btn>
                </template>

                <v-list>
                    <v-list-item>
                    <v-list-item-title></v-list-item-title>
                    </v-list-item>
                </v-list>
                </v-menu>
            </div>
            <div class="menu-item">
                <v-menu open-on-hover bottom offset-y>
                <template v-slot:activator="{ on }">
                    <v-btn
                    text
                    small
                    color="#104388"
                    v-on="on"
                    >
                    Our community
                    <v-icon right dark>mdi-menu-down</v-icon>
                    </v-btn>
                </template>
                <v-list>
                    <v-list-item>
                    <v-list-item-title></v-list-item-title>
                    </v-list-item>
                </v-list>
                </v-menu>
            </div>
            <div class="menu-item">
                <v-menu open-on-hover bottom offset-y>
                <template v-slot:activator="{ on }">
                    <v-btn
                    small
                    color="#104388"
                    class="ma-2 white--text"
                    v-on="on"
                    >
                    Login
                    <v-icon right dark>mdi-menu-down</v-icon>
                    </v-btn>
                </template>

                <v-list>
                    <v-list-item>
                    <v-list-item-title></v-list-item-title>
                    </v-list-item>
                </v-list>
                </v-menu>
            </div>
            <div class="menu-item">
                <v-menu open-on-hover bottom offset-y>
                <template v-slot:activator="{ on }">
                    <v-btn
                    small
                    color="#24b149"
                    class="ma-2 white--text"
                    v-on="on"
                    >
                    Join now
                    <v-icon right dark>mdi-menu-down</v-icon>
                    </v-btn>
                </template>

                <v-list>
                    <v-list-item>
                    <v-list-item-title></v-list-item-title>
                    </v-list-item>
                </v-list>
                </v-menu>
            </div>
            <div class="menu-item">
                <v-menu open-on-hover bottom offset-y>
                <template v-slot:activator="{ on }">
                    <v-btn
                    small
                    color="#b18b24"
                    class="ma-2 white--text"
                    v-on="on"
                    >
                    Lists
                    <v-icon right dark>mdi-menu-down</v-icon>
                    </v-btn>
                </template>

                <v-list>
                    <v-list-item>
                    <v-list-item-title></v-list-item-title>
                    </v-list-item>
                </v-list>
                </v-menu>
            </div>
      </v-toolbar-items>
      <v-toolbar  @click.stop="drawer = !drawer" class="hidden-md-and-up"><v-icon>mdi-menu</v-icon></v-toolbar>
    </v-toolbar>
        <v-navigation-drawer
        v-model="drawer"
        absolute
        temporary
        >
            <v-list>
                <v-list-group
                    value="true"
                >
                    <template v-slot:activator>
                    <v-list-item-title>How it works</v-list-item-title>
                    </template>
                </v-list-group>
                <v-list-group
                    value="true"
                >
                    <template v-slot:activator>
                    <v-list-item-title>Our community</v-list-item-title>
                    </template>
                </v-list-group>
                <v-list-group
                    value="true"
                >
                    <template v-slot:activator>
                    <v-list-item-title>Login</v-list-item-title>
                    </template>
                </v-list-group>
                <v-list-group
                    value="true"
                >
                    <template v-slot:activator>
                    <v-list-item-title>Join now</v-list-item-title>
                    </template>
                </v-list-group>
                <v-list-group
                    value="true"
                >
                    <template v-slot:activator>
                    <v-list-item-title>Lists</v-list-item-title>
                    </template>
                </v-list-group>
            </v-list>
        </v-navigation-drawer>
    </div>
</template>

<script>
export default {
  data ( ) {
      return{
        drawer: null 
      }
  }
}
</script>

<style scoped>
    .menu-item{
        margin: auto;
    }
    .menu-item .v-btn.v-size--small{
        text-transform: unset;
        font-size: 14px;
        font-weight: 600;
    }
    .menu-item .v-btn > .v-btn__content .v-icon {
        margin: 2px 0px 0 3px;
        font-size: 26px;
    }
    
    @media (max-width: 1023px) {
        .head-logo img{
            width:180px;
        }
        .hidden-md-and-up {
            box-shadow: unset;
        }
        .hidden-md-and-up .v-icon.v-icon{
            margin-left: auto;
        }

    }
</style>










