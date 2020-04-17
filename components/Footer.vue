<template>
  <v-footer
    dark
    class="let-foot" >
  <div class="footer-top">
    <v-container>
        <v-row>
            <v-col cols="12" md="3" sm="6">
                <v-list>
                    <v-subheader>How Letme-save.com works</v-subheader>
                        <v-list-item>Information for food partners</v-list-item>
                        <v-list-item>Information for users</v-list-item>
                        <v-list-item>Information for marketing partners</v-list-item>
                        <v-list-item>Green awareness</v-list-item>
                        <v-list-item>Food alergies</v-list-item>
                        <v-list-item>FAQ</v-list-item>
                </v-list>
            </v-col>
            <v-col cols="12" md="3" sm="6">
                <v-list>
                    <v-subheader>Our community</v-subheader>
                
                        <v-list-item>Find food</v-list-item>
                        <v-list-item>Find offers</v-list-item>
                        <v-list-item>Blog</v-list-item>
                        <v-list-item>Becomes our ambassadors</v-list-item>
                        <v-list-item>Gallery</v-list-item>
                        <v-list-item>Our mission</v-list-item>
                        <v-list-item>Contact Us</v-list-item>
                </v-list>
            </v-col>
            <v-col cols="12" md="3" sm="6">
                <v-list>
                    <v-subheader>Login as a</v-subheader>
                
                        <v-list-item>Food partner</v-list-item>
                        <v-list-item>User </v-list-item>
                        <v-list-item>Marketing partner</v-list-item>
                        <v-list-item>Host</v-list-item>
                        <v-list-item>Volunteer</v-list-item>

                    <v-subheader style="margin-top:20px;">Join now as a</v-subheader>
                        <v-list-item>Food partner</v-list-item>
                        <v-list-item>User </v-list-item>
                        <v-list-item>Marketing partner</v-list-item>
                        <v-list-item>Host</v-list-item>
                        <v-list-item>Volunteer</v-list-item>
                </v-list>
            </v-col>
            <v-col cols="12" md="3" sm="6">
                <v-list>
                    <v-subheader>Legal</v-subheader>
                        <v-list-item>Terms and conditions</v-list-item>
                        <v-list-item>Data and privacy policy</v-list-item>

                    <v-subheader style="margin-top:20px;">Follow us on</v-subheader>
                        <v-list-item><v-icon>mdi-facebook</v-icon><v-icon>mdi-twitter</v-icon><v-icon>mdi-instagram</v-icon></v-list-item>
                        
                </v-list>
            </v-col>
        </v-row>
    </v-container>
  </div>
  <v-divider></v-divider>
  <div class="footer-bottom">
    <v-row>
        
        <v-col cols="12" sm="6">
            <div class="copyy">Copyright &copy; {{ new Date().getFullYear() }} Letme-save.com. All rights reserved.</div>
        </v-col>
        <v-col cols="12" sm="6">
            <div class="designn">
                Designed by
                <a href="https://imaginetventures.com" target="_blank">ImagiNET Ventures</a>
            </div>
        </v-col>
    </v-row>
  </div>
  
  </v-footer>
  
</template>

<style scoped>
.theme--dark.v-footer {
    background-color: #282c2f;
}
.footer-top .theme--dark.v-list {
    background: unset;
}
.footer-top .v-list-item{
    min-height:unset ;
    font-size: 14px;
}
.footer-top .v-subheader{
    font-size: 15px;
    color: #fff;
    font-weight: 500;
    height: 40px;
}
.footer-top{
    width:100%;
}
.footer-bottom{
    padding: 20px;
    width: 100%;
    border-top: 1px solid #ffffff38;
}
.designn{
    text-align: right;
}
a{
    text-decoration: none;
    color: unset;
}
.footer-top .v-icon.v-icon{
    margin: 0 10px 0 0;
}
@media (max-width: 767px){
    .copyy, .designn{
        text-align: left;
    }

}
</style>