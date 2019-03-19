<template>
  <v-container>
    <v-layout text-xs-center wrap>
      <v-flex mb-4>
        <h1 class="display-2 font-weight-bold mb-3">
          Welcome
        </h1>
        <p class="subheading font-weight-regular">
          Demo proto type template here.
        </p>
      </v-flex>

      <v-flex mb-5 xs12>
        <h2 class="headline font-weight-bold mb-3">What's next?</h2>
        <p class="subheading font-weight-regular">
          Give me some feedback!
        </p>
      </v-flex>

      <v-flex xs12 sm6 d-flex>
        <v-select :items="items" label="Finding"></v-select>
      </v-flex>

      <v-flex xs12>
        <v-combobox
          v-model="select"
          :items="combo_items"
          label="Select an amount or create a new one"
        ></v-combobox>
      </v-flex>

      <v-flex xs12>
        <v-combobox
          v-model="select"
          :items="take_notes_items"
          label="Take notes of"
        ></v-combobox>
      </v-flex>

      <v-flex xs12>
        <v-combobox
          v-model="select"
          :items="segment_items"
          label="Select a location segment"
        ></v-combobox>
      </v-flex>

      <v-flex xs12>
        <v-combobox
          v-model="select"
          :items="orientation_items"
          label="Select a location orientation"
        ></v-combobox>
      </v-flex>

      <v-flex xs12 sm6 md3>
        <v-text-field label="Size (cm)"></v-text-field>
      </v-flex>

      <v-flex xs12>
        <v-combobox
          v-model="select"
          :items="intervention_items"
          label="Select an intervention item"
        ></v-combobox>
      </v-flex>

      <v-flex xs12>
        <v-textarea
          outline
          name="input-7-4"
          label="Generated text"
          v-model="result_text"
        ></v-textarea>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    items: ["Polyp", "Lymphoid hyperplasia-terminal ileum"],
    combo_items: ["1", "several", "multiple"],
    take_notes_items: ["the most significant", "each", "overall"],
    segment_items: [
      "Terminal ileum",
      "Cecum",
      "Ascending colon",
      "Hepatic flexure",
      "Transverse colon",
      "Splenic flexure",
      "Descending colon",
      "Sigmoid colon",
      "RS junction",
      "Rectum",
      "All segments of colon",
      "Anastomosis"
    ],
    orientation_items: [
      "<none>",
      "proximal",
      "middle",
      "distal",
      "upper",
      "lower"
    ],
    intervention_items: ["Biopsy", "Polypectomy", "EMR", "ESD"],
    result_text:
      "(83) (87)colon  polyp/polyps(視83單複數), (86)(可以是range), (88)，(89-t), (90-t), (91-t),  at the (85)location(可多選) was/were found. s/p (92)",
    ecosystem: [
      {
        text: "vuetify-loader",
        href: "https://github.com/vuetifyjs/vuetify-loader"
      },
      {
        text: "github",
        href: "https://github.com/vuetifyjs/vuetify"
      },
      {
        text: "awesome-vuetify",
        href: "https://github.com/vuetifyjs/awesome-vuetify"
      }
    ],
    importantLinks: [
      {
        text: "Documentation",
        href: "https://vuetifyjs.com"
      },
      {
        text: "Chat",
        href: "https://community.vuetifyjs.com"
      },
      {
        text: "Made with Vuetify",
        href: "https://madewithvuetifyjs.com"
      },
      {
        text: "Twitter",
        href: "https://twitter.com/vuetifyjs"
      },
      {
        text: "Articles",
        href: "https://medium.com/vuetify"
      }
    ],
    whatsNext: [
      {
        text: "Explore components",
        href: "https://vuetifyjs.com/components/api-explorer"
      },
      {
        text: "Select a layout",
        href: "https://vuetifyjs.com/layout/pre-defined"
      },
      {
        text: "Frequently Asked Questions",
        href: "https://vuetifyjs.com/getting-started/frequently-asked-questions"
      }
    ]
  })
};
</script>

<style>
</style>
