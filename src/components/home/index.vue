<template>
    <div >
        <template>
          <v-btn @click="goRoute()" color="green">+ nova compra</v-btn>
            <v-simple-table>
              
                <template v-slot:default>
                
                <thead>
                    <tr>
                      <th class="text-left">
                        n° Pedido
                      </th>

                      <th class="text-left">
                        N° nota(s)
                      </th>

                      <th class="text-left">
                        Fornecedor
                      </th>

                      <th class="text-left">
                        Entrega
                      </th>

                      <th class="text-left">
                        Pagamento
                      </th>
                      
                      <th class="text-center">
                        Ações
                      </th>
                    </tr>
                </thead>

                <tbody>
                    <tr
                    v-for="item in desserts"
                    :key="item.name"
                    >
                      <td>1</td>
                      <td>
                        <v-btn v-if="isMultipleNote()" icon>
                          <v-tooltip bottom>
                            <template v-slot:activator="{ on, attrs }">
                              <v-icon
                                color="primary"
                                dark
                                v-bind="attrs"
                                v-on="on"
                              >
                                mdi-text-box-multiple-outline
                              </v-icon>
                            </template>

                            <span>Ver lista de notas</span>
                          </v-tooltip>
                        </v-btn>

                        <span v-if="!isMultipleNote()">
                          N° nota(s)

                          <v-btn icon>
                            <v-tooltip bottom>
                              <template v-slot:activator="{ on, attrs }">
                                <v-icon
                                  color="primary"
                                  dark
                                  v-bind="attrs"
                                  v-on="on"
                                >
                                  mdi-note-search-outline
                                </v-icon>
                              </template>

                              <span>Ver nota</span>
                            </v-tooltip>
                        </v-btn>
                        </span>
                      </td>
                      <td>nome do fornecedor</td>
                      <td>status</td>

                      <td>status</td>

                      <td class="text-center">
                        

                        <v-btn icon>
                          <v-tooltip bottom>
                            <template v-slot:activator="{ on, attrs }">
                              <v-icon
                                color="primary"
                                dark
                                v-bind="attrs"
                                v-on="on"
                              >
                                mdi-text-box-search-outline
                              </v-icon>
                            </template>

                            <span>Ver pedido</span>
                          </v-tooltip>
                        </v-btn>

                        <v-btn icon>
                          <v-tooltip bottom>
                            <template v-slot:activator="{ on, attrs }">
                              <v-icon
                                color="primary"
                                dark
                                v-bind="attrs"
                                v-on="on"
                              >
                                mdi-text-box-edit-outline
                              </v-icon>
                            </template>

                            <span>Editar pedido</span>
                          </v-tooltip>
                        </v-btn>
                      </td>
                    </tr>
                </tbody>
                </template>
            </v-simple-table>
        </template>
    </div>
</template>

<script>
export default {
  name: 'Home',

  props: {
      msg: String
  },

  data: () => ({
      teste:'teste 123 33423423',
      desserts: [
        {
          name: 'Frozen Yogurt',
          calories: 159,
        },
        {
          name: 'Ice cream sandwich',
          calories: 237,
        },
        {
          name: 'Eclair',
          calories: 262,
        },
        {
          name: 'Cupcake',
          calories: 305,
        },
        {
          name: 'Gingerbread',
          calories: 356,
        },
        {
          name: 'Jelly bean',
          calories: 375,
        },
        {
          name: 'Lollipop',
          calories: 392,
        },
        {
          name: 'Honeycomb',
          calories: 408,
        },
        {
          name: 'Donut',
          calories: 452,
        },
        {
          name: 'KitKat',
          calories: 518,
        },
      ],
  }),

  methods:{
    goRoute(){
      this.router.push({ name: 'purchase' })
    },

    isMultipleNote(){
      return true
    },
    
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
  