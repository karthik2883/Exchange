 <template>
  <v-container fluid>
    <v-layout dark row>
      <v-flex xs4>
        <v-card>
          <v-data-table :headers="headers" :items="desserts" class="elevation-1">
            <template slot="items" slot-scope="props">
              <td>{{ props.item.name }}</td>
              <td class="text-xs-right">{{ props.item.calories }}</td>
              <td class="text-xs-right">{{ props.item.fat }}</td>
              <td class="text-xs-right">{{ props.item.carbs }}</td>
              <td class="text-xs-right">{{ props.item.protein }}</td>
              <td class="text-xs-right">{{ props.item.iron }}</td>
            </template>
          </v-data-table>
        </v-card>
      </v-flex>
      <v-flex grow pa-1>
        <v-card dark color="black darken-1">
          <v-card-text>#1 Im a Grow Flex</v-card-text>
        </v-card>
      </v-flex>
      <v-flex xs4>
        <v-card dark color="black darken-3">
          <v-card-text>#1 Im a Grow Flex</v-card-text>
          <v-card-text>#1 Im a Grow Flex</v-card-text>
          <v-card-text>#1 Im a Grow Flex</v-card-text>
          <v-card-text>#1 Im a Grow Flex</v-card-text>
          <v-card-text>#1 Im a Grow Flex</v-card-text>
          <v-card-text>#1 Im a Grow Flex</v-card-text>
        </v-card>
      </v-flex>
    </v-layout>
    <v-layout row>
      <v-flex shrink pa-1>
        <v-card dark color="black darken-3">
          <v-card-text>#1 Im a Grow Flex</v-card-text>
          <v-card-text>#1 Im a Grow Flex</v-card-text>
          <v-card-text>#1 Im a Grow Flex</v-card-text>
          <v-card-text>#1 Im a Grow Flex</v-card-text>
          <v-card-text>#1 Im a Grow Flex</v-card-text>
          <v-card-text>#1 Im a Grow Flex</v-card-text>
        </v-card>
      </v-flex>
    </v-layout>
    <v-layout row>
      <v-flex grow pa-1>
        <v-card dark color="green darken-1">
          <v-card-text>#1 Im a Grow Flex</v-card-text>
        </v-card>
      </v-flex>
      <v-flex shrink pa-1>
        <v-card dark color="green lighten-1">
          <v-card-text>#2 Im a Shrink Flex</v-card-text>
        </v-card>
      </v-flex>
      <v-flex grow pa-1>
        <v-card dark color="green darken-4">
          <v-card-text>#3 Im a Grow Flex</v-card-text>
        </v-card>
      </v-flex>
    </v-layout>
    <v-layout row>
      <v-flex shrink pa-1>
        <v-card dark color="green darken-3">
          <v-card-text>#1 Im a Shrink Flex</v-card-text>
        </v-card>
      </v-flex>
      <v-flex grow pa-1>
        <v-card dark color="green">
          <v-card-text>#2 Im a Grow Flex</v-card-text>
        </v-card>
      </v-flex>
      <v-flex shrink pa-1>
        <v-card dark color="green lighten-1">
          <v-card-text>#3 Im a Shrink Flex</v-card-text>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

 <script>
export default {
    data() {
        return {
            headers: [
                {
                    text: 'Dessert (100g serving)',
                    align: 'left',
                    sortable: false,
                    value: 'name'
                },
                { text: 'Calories', value: 'calories' },
                { text: 'Fat (g)', value: 'fat' },
                { text: 'Carbs (g)', value: 'carbs' },
                { text: 'Protein (g)', value: 'protein' },
                { text: 'Iron (%)', value: 'iron' }
            ],
            desserts: [
                {
                    name: 'Frozen Yogurt',
                    calories: 159,
                    fat: 6.0,
                    carbs: 24,
                    protein: 4.0,
                    iron: '1%'
                },
                {
                    name: 'Ice cream sandwich',
                    calories: 237,
                    fat: 9.0,
                    carbs: 37,
                    protein: 4.3,
                    iron: '1%'
                },
                {
                    name: 'Eclair',
                    calories: 262,
                    fat: 16.0,
                    carbs: 23,
                    protein: 6.0,
                    iron: '7%'
                },
                {
                    name: 'Cupcake',
                    calories: 305,
                    fat: 3.7,
                    carbs: 67,
                    protein: 4.3,
                    iron: '8%'
                },
                {
                    name: 'Gingerbread',
                    calories: 356,
                    fat: 16.0,
                    carbs: 49,
                    protein: 3.9,
                    iron: '16%'
                },
                {
                    name: 'Jelly bean',
                    calories: 375,
                    fat: 0.0,
                    carbs: 94,
                    protein: 0.0,
                    iron: '0%'
                },
                {
                    name: 'Lollipop',
                    calories: 392,
                    fat: 0.2,
                    carbs: 98,
                    protein: 0,
                    iron: '2%'
                },
                {
                    name: 'Honeycomb',
                    calories: 408,
                    fat: 3.2,
                    carbs: 87,
                    protein: 6.5,
                    iron: '45%'
                },
                {
                    name: 'Donut',
                    calories: 452,
                    fat: 25.0,
                    carbs: 51,
                    protein: 4.9,
                    iron: '22%'
                },
                {
                    name: 'KitKat',
                    calories: 518,
                    fat: 26.0,
                    carbs: 65,
                    protein: 7,
                    iron: '6%'
                }
            ]
        };
    }
};
</script>
<style scoped>
</style>
