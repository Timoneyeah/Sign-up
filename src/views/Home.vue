<template>
  <v-container>
    <v-row align="center" justify="center">
      <v-col cols="12" sm="10">
        <v-card class="elevation-6 mt-10">
          <v-window v-model="step">
            <v-window-item :value="1">
              <v-row>
                <v-col cols="12" sm="6">
                  <v-card-text class="mt-12">
                    <h4  class="text-center">Login in to Your Account</h4>
                    <h6 class="text-center purple--text" style="font-size: 13px;">Login in to your account so you can continue building your account 
                      <br> and editing your onboarding flows
                    </h6>
                    <v-row align="center" justify="center">
                      <v-col cols="12" sm="8">
                        <v-text-field label="Email" outlined dense color="blue" autocomplete="false" class="mt-16"></v-text-field>
                        <v-text-field label="Password" outlined dense color="blue" autocomplete="false" type="password"></v-text-field>
                        <v-row>
                          <v-col cols="12" sm="7">
                            <v-checkbox label="Remember Me" class="mt-n1" color="blue"></v-checkbox>
                          </v-col>
                          <v-col cols="12" sm="5">
                            <span class="caption blue--text" style="cursor: pointer;">Forget Password</span>
                          </v-col>
                        </v-row>
                        <v-btn color="blue" dark block tile>Login in</v-btn>
                        <h5 class="text-center purple--text mt-4 mb-3">Or Log in using</h5>
                        <div class="d-flex justify-space-between align-center mx-10 mb-16">
                          <v-btn depressed outlined color="orange">
                            <v-icon color="red">fab fa-google fa-bounce  </v-icon>
                          </v-btn>
                          <v-btn depressed outlined color="blue">
                            <v-icon style="font-size: 30px;"  color="blue">fab fa-facebook fa-beat </v-icon>
                          </v-btn>

                          <v-btn depressed outlined color="pink">
                            <v-icon style="font-size: 30px;" color="pink">fab fa-instagram fa-spin </v-icon>
                          </v-btn>
                         
                        </div>
                        
                      </v-col>
                    </v-row>
                  </v-card-text>
                </v-col>
                <v-col cols="12" sm="6" class="blue rounded-bl-xl ">
                  <div style="text-align:center; padding: 180px 0;">
                    <v-card-text class="white--text">
                      <h3 class="text-center">Don't have an Account Yet?</h3>
                      <h6 style="font-size: 13px; color: yellow;" class="text-center">
                        Let's get you all set up so you can start creating your first <br>
                        onboarding experience
                      </h6>
                    </v-card-text>
                    <div class="text-center">
                      <v-btn tile outlined dark @click="step++">SIGN UP</v-btn>
                    </div>
                  </div>
                </v-col>
                
              </v-row>
            </v-window-item>
            <v-window-item :value="2">
              <v-row>
                <v-col cols="12" sm="6" class="blue rounded-br-xl">
                  <div style="text-align:center; padding: 180px 0;">
                    <v-card-text class="white--text">
                      <h3 class="text-center">Already Signed Up?</h3>
                      <h6 style="font-size: 13px; color: yellow;" class="text-center">SignLog in to your account so you can continue building and <br>
                      editing your onboarding flows
                      </h6>
                    </v-card-text>
                    <div class="text-center">
                      <v-btn tile outlined dark @click="step--">Log in</v-btn>
                    </div>

                  </div>
                </v-col>
                <v-col cols="12" sm="6">
                  <v-card-text class="mt-12">
                    <h4 class="text-center">Sign up for an Account</h4>
                    <h6 style="font-size: 13px;" class="text-center purple--text">
                      Let's get you all set up so you can start creation your <br>
                      first onboarding experience
                    </h6>
                    <v-row align="center" justify="center">
                      <v-col cols="12" sm="8">
                        <v-row>
                          <v-col cols="12" sm="6">
                            <v-text-field label="First Name" outlined dense color="blue" autocomplete="false" class="mt-4"></v-text-field>

                          </v-col>
                          <v-col cols="12" sm="6">
                            <v-text-field label="Last Name" outlined dense color="blue" autocomplete="false" class="mt-4"></v-text-field>
                          </v-col>
                        </v-row>
                        <v-text-field label="Email" outlined dense color="blue" autocomplete="false"></v-text-field>
                        <v-text-field label="Password" outlined dense color="blue" type="password"></v-text-field>
                        <v-row>
                          <v-col cols="12" sm="7">
                            <v-checkbox label="I Accept Timoney" class="mt-n1" color="blue"></v-checkbox>
                          </v-col>
                          <v-col cols="12" sm="5">
                            <span class="caption blue--text ml-n4">Terms & Conditions</span>
                          </v-col>
                        </v-row>
                        <v-btn color="blue" dark block tile>Sign Up</v-btn>
                        <h5 class="text-center purple--text mt-4 mb-3">Dr Sign up using</h5>
                        <div class="d-flex justify-space-between align-center mx-10 mb-11">
                          <v-btn depressed outlined color="purple">
                            <v-icon color="red">fa-brands fa-google fa-bounce</v-icon>
                          </v-btn>
                          <v-btn depressed outlined color="blue">
                            <v-icon style="font-size: 28px;" color="blue">fa-brands fa-telegram fa-beat</v-icon>
                          </v-btn>
                          <v-btn depressed outlined color="green">
                            <v-icon style="font-size: 28px;" color="light-blue lighteen-3">fa-brands fa-linkedin  fa-shake</v-icon>
                          </v-btn>
                        </div>
                      </v-col>
                    </v-row>
                  </v-card-text>
                </v-col>
              </v-row>
            </v-window-item>
          </v-window>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  

  export default {
    data: () =>({
      step: 1
    }),
    propos: {
      source: String
    }

    
  }
</script>

<style scoped>
.v-application .rounded-bl-xl{
  border-bottom-left-radius: 300px !important;

}
.v-application .rounded-br-xl {
  border-bottom-right-radius: 300px !important;
}

</style>
