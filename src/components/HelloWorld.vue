<template>
  <v-container grid-list-md fluid>
    <v-layout align-center justify-center>
      <v-flex xs12 sm6>
            <v-layout wrap align-center justify-center>
              <v-flex
                v-for="n in 9"
                :key="n"
                xs4
              >
                  <v-btn v-if="n%2" fab dark large :color="values[n].color">
                    <v-icon dark>{{values[n].icon}}</v-icon>
                  </v-btn>
              </v-flex>
            </v-layout>
      </v-flex>
    </v-layout>
  </v-container>

  <!-- <v-layout align-center justify-center>
    <v-flex xs12 sm6 offset-sm3>
        <v-container grid-list-md fluid>
          <v-layout row wrap align-center justify-center>
            <v-flex
              v-for="n in 9"
              :key="n"
              xs4
            >
                <v-btn v-if="n%2" fab dark large color="purple">
                  <v-icon dark>android</v-icon>
                </v-btn>
            </v-flex>
          </v-layout>
        </v-container>
    </v-flex>
  </v-layout> -->

</template>

<script>
  export default {
    data: () => ({
      values: [
        {color: "#2de348", icon: "android"},
        {color: "#5b56b8", icon: "store"},
        {color: "#3c6446", icon: "cancel"},
        {color: "#fbf88c", icon: "attach_money"},
        {color: "#cf0a3c", icon: "android"},
        {color: "#87816b", icon: "cancel"},
        {color: "#0225c8", icon: "android"},
        {color: "#cd6a49", icon: "accessibility"},
        {color: "#6bbb24", icon: "android"},
        {color: "#6245b8", icon: "android"}
      ]


    })
  }
</script>