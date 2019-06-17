<template>
  <v-container>
    <v-layout row wrap>
      <v-flex xs12 sm6 md6 lg4 class="pa-4">
        <v-card hover class="projCard">
          <div>
            <h1 class="text-xs-center pa-3 pt-5">Project Ideas</h1>
            <v-divider style="margin: 0 auto; width: 90%; margin-bottom: 20px;"></v-divider>
          </div>

          <v-list
            two-line
            class="pa-2 mt-2 item-card"
            v-for="(project, index) in projectIdeas"
            :key="index"
            hover
          >
            <template class="pa-2">
              <v-list-tile>
                <v-list-tile-avatar>
                  <v-icon medium color="black">assignment</v-icon>
                </v-list-tile-avatar>

                <v-list-tile-content>
                  <v-list-tile-title>{{project.name}}</v-list-tile-title>
                  <v-list-tile-sub-title>{{project.description}}</v-list-tile-sub-title>
                </v-list-tile-content>
              </v-list-tile>
            </template>
          </v-list>
        </v-card>
      </v-flex>

      <v-flex xs12 sm6 md6 lg4 class="pa-4">
        <v-card hover class="projCard">
          <div>
            <h1 class="text-xs-center pa-3 pt-5">Current Projects</h1>
            <v-divider style="margin: 0 auto; width: 90%; margin-bottom: 20px;"></v-divider>
          </div>

          <v-card-title
            primary-title
            v-for="(project, index) in currentProjects"
            :key="index"
            class="pa-2"
          >
            <v-list two-line class="pa-0 item-card">
              <v-card hover class="item-card">
                <template>
                  <v-list-tile>
                    <v-list-tile-avatar>
                      <v-icon medium color="black">assignment</v-icon>
                    </v-list-tile-avatar>

                    <v-list-tile-content>
                      <v-list-tile-title>{{project.name}}</v-list-tile-title>
                      <v-list-tile-sub-title>{{project.description}}</v-list-tile-sub-title>
                    </v-list-tile-content>
                  </v-list-tile>
                </template>
              </v-card>
            </v-list>
          </v-card-title>
        </v-card>
      </v-flex>

      <v-flex xs12 sm6 md6 lg4 class="pa-4">
        <v-card hover class="projCard">
          <div>
            <h1 class="text-xs-center pa-3 pt-5">Launched Projects</h1>
            <v-divider style="margin: 0 auto; width: 90%; margin-bottom: 20px;"></v-divider>
          </div>

          <v-card-title
            primary-title
            v-for="(project, index) in launchedProjects"
            :key="index"
            class="pa-2"
          >
            <v-list two-line class="pa-0 item-card">
              <v-card hover class="item-card">
                <template>
                  <v-list-tile>
                    <v-list-tile-avatar>
                      <v-icon medium color="black">assignment</v-icon>
                    </v-list-tile-avatar>

                    <v-list-tile-content>
                      <v-list-tile-title>{{project.name}}</v-list-tile-title>
                      <v-list-tile-sub-title>{{project.description}}</v-list-tile-sub-title>
                    </v-list-tile-content>
                  </v-list-tile>
                </template>
              </v-card>
            </v-list>
          </v-card-title>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      projectIdeas: [
        {
          name: "Todo-app",
          description: "An app to set up and complete your todos"
        },
        {
          name: "Recipe-Grocery-App",
          description:
            "Save your recipes, add them to your grocery-list whenever you head to the store to get quick access to the ingredients needed"
        }
      ],
      currentProjects: [
        {
          name: "Todo-app",
          description: "An app to set up and complete your todos"
        },
        {
          name: "Recipe-Grocery-App",
          description:
            "Save your recipes, add them to your grocery-list whenever you head to the store to get quick access to the ingredients needed"
        }
      ],
      launchedProjects: [
        {
          name: "Todo-app",
          description: "An app to set up and complete your todos"
        },
        {
          name: "Recipe-Grocery-App",
          description:
            "Save your recipes, add them to your grocery-list whenever you head to the store to get quick access to the ingredients needed"
        },
        {
          name: "Todo-app",
          description: "An app to set up and complete your todos"
        },
        {
          name: "Recipe-Grocery-App",
          description:
            "Save your recipes, add them to your grocery-list whenever you head to the store to get quick access to the ingredients needed"
        },
        {
          name: "Todo-app",
          description: "An app to set up and complete your todos"
        },
        {
          name: "Recipe-Grocery-App",
          description:
            "Save your recipes, add them to your grocery-list whenever you head to the store to get quick access to the ingredients needed"
        }
      ]
    };
  }
};
</script>
<style scoped>
div.v-card.projCard {
  background: linear-gradient(157deg, #f0f3f5 50%, #9bb4c1 50.2%);
  min-height: 500px;
}
div.item-card {
  border-radius: 5px;
  background: rgba(255, 255, 255, 0.9);
  width: 90%;
  margin: 0 auto;
}
</style>
