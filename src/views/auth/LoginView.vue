<!--Programming naming conventions-->
<script setup>
//import { useDisplay } from 'vuetify'
import '@/assets/login_style.css'
import LoginForm from '@/components/auth/LoginForm.vue'
import '@/assets/theme_style.css'

//const { mobile } = useDisplay()

//import { ref } from 'vue'
</script>

<template>
  <v-responsive>
    <v-container-fluid>
      <v-row style="height: 100vh; margin: 0; padding: 0"
        ><v-col class="container">
          <v-card
            elevation="24"
            class="mx-auto rounded-xl bg-grey-darken-4"
            style="margin-top: 15vh"
            width="70%"
          >
            <v-row>
              <v-col>
                <v-container>
                  <video
                    class="background-video"
                    autoplay
                    loop
                    muted
                    :src="'/template-video/girl2.mp4'"
                  ></video>
                  <v-row class="fill-height"></v-row>
                </v-container>
              </v-col>

              <v-col>
                <v-card class="bg-grey-darken-4 custom-card-container">
                  <v-card-title>
                    <v-container>
                      <h2 id="font_welcome" class="font-weight-medium">Welcome Back!</h2>
                      <small>Sign in to your account</small>
                    </v-container>
                  </v-card-title>

                  <v-sheet class="mx-auto bg-transparent" width="85%">
                    <LoginForm> </LoginForm>
                    <v-divider class="my-4 border-opacity-25"></v-divider>
                    <h6 class="my-3 text-center">
                      Don't have an account?
                      <RouterLink to="/register" class="text-primary" style="text-decoration: none"
                        >Sign up here<v-icon icon="mdi-chevron-right"></v-icon
                      ></RouterLink>
                    </h6>
                  </v-sheet>

                  <v-footer class="footer-text font-weight-light my-2"
                    >Copyright © 2024. All rights reserved</v-footer
                  >
                </v-card>

                <!--logo-Title-->

                <v-card-title class="text-center logo-position">
                  <v-img
                    src="/images/logo.png"
                    alt="Logo"
                    :width="mobile ? '75%' : '45%'"
                    class="d-block mx-auto"
                    draggable="false"
                    style="user-select: none"
                  ></v-img>
                  <p id="cam_font" class="text-center">CAM'N GO</p>
                  <small><i>Unleash your wildest angles with Cam’n Go</i></small>
                </v-card-title>
              </v-col>
            </v-row>
          </v-card>
        </v-col></v-row
      >
    </v-container-fluid>
  </v-responsive>
</template>
