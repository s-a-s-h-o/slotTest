<template>
  <appWrapper>
    <div slot="head">
      <headerTest/>
    </div>
    <div slot="messageBox">
      <!-- <testThree/> -->
      <div>
        <div class="text-xs-center">
          <v-btn color="primary" @click="alert = !alert">Toggle</v-btn>
        </div>
        <v-alert
          :value="alert"
          type="success"
          transition="scale-transition"
        >This is a success alert.</v-alert>
      </div>
    </div>
    <div slot="body">
      <v-flex xs12 sm6 offset-sm3>
        <v-card>
          <v-img src="https://cdn.vuetifyjs.com/images/cards/desert.jpg" aspect-ratio="2.75"></v-img>

          <v-card-title primary-title>
            <div>
              <h3 class="headline mb-0">Kangaroo Valley Safari</h3>
              <div>{{ card_text }}</div>
            </div>
          </v-card-title>

          <v-card-actions>
            <v-btn flat color="orange">Share</v-btn>
            <v-btn flat color="orange">Explore</v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
      <v-flex xs12 sm6 offset-sm3>
        <v-card>
          <v-img src="https://cdn.vuetifyjs.com/images/cards/desert.jpg" aspect-ratio="2.75"></v-img>

          <v-card-title primary-title>
            <div>
              <h3 class="headline mb-0">Kangaroo Valley Safari</h3>
              <div>{{ card_text }}</div>
            </div>
          </v-card-title>

          <v-card-actions>
            <v-btn flat color="orange">Share</v-btn>
            <v-btn flat color="orange">Explore</v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
      <v-flex xs12 sm6 offset-sm3>
        <v-card>
          <v-img src="https://cdn.vuetifyjs.com/images/cards/desert.jpg" aspect-ratio="2.75"></v-img>

          <v-card-title primary-title>
            <div>
              <h3 class="headline mb-0">Kangaroo Valley Safari</h3>
              <div>{{ card_text }}</div>
            </div>
          </v-card-title>

          <v-card-actions>
            <v-btn flat color="orange">Share</v-btn>
            <v-btn flat color="orange">Explore</v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
      <v-flex xs12 sm6 offset-sm3>
        <v-card>
          <v-img src="https://cdn.vuetifyjs.com/images/cards/desert.jpg" aspect-ratio="2.75"></v-img>

          <v-card-title primary-title>
            <div>
              <h3 class="headline mb-0">Kangaroo Valley Safari</h3>
              <div>{{ card_text }}</div>
            </div>
          </v-card-title>

          <v-card-actions>
            <v-btn flat color="orange">Share</v-btn>
            <v-btn flat color="orange">Explore</v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
    </div>
    <div class="footerWrapper" slot="footer">
      <v-footer class="pa-3">
        <v-spacer></v-spacer>
        <div>&copy; {{ new Date().getFullYear() }}</div>
      </v-footer>
    </div>
  </appWrapper>
</template>

<script>
import appWrapper from "../components/appWrapper";
import headerTest from "../components/headerTest";
import testThree from "../components/testThree";

export default {
  components: {
    appWrapper,
    headerTest,
    testThree
  },
  data() {
    return {
      alert: true,
      card_text:"custom text"
    };
  },
  mounted() {
    console.log("this.$vuetify.theme", this.$vuetify.theme);
  }
};
</script>

<style>
.flex {
  padding: 10px;
}
.footerWrapper .v-footer {
  background: green;
  padding: 20px !important;
  height: 100px !important;
}
</style>
