<template>
  <div >
    <v-form>
      <v-container>

        <v-row>
          titulo pedido
          <v-col
            md="3"
          >
            <v-text-field
              label="Numero"
            ></v-text-field>
          </v-col>
          
          <v-col
            md="3"
          >
            <v-text-field
              label="Data de emissao"
            ></v-text-field>
          </v-col>

          
          <v-col
            md="3"
          >
            <v-text-field
              label="Previsão de entrega"
            ></v-text-field>
          </v-col>

          
          <v-col
            md="3"
          >
            <v-text-field
              label="loja"
            ></v-text-field>
          </v-col>

          
          <v-col
            md="3"
          >
            <v-text-field
              label="Solicitante"
            ></v-text-field>
          </v-col>

          
          <v-col
            md="3"
          >
            <v-text-field
              label="contato"
            ></v-text-field>
          </v-col>
        </v-row>


        <v-row>
          titulo fornecedor


          <v-col
            md="3"
          >
            <v-text-field
              label="Fornecedor(input)"
            ></v-text-field>
          </v-col>

          <v-col
            md="3"
          >
            <v-text-field
              label="serie(input)"
            ></v-text-field>
          </v-col>

          <v-col
            md="3"
          >
            <v-text-field
              label="numero(input)"
            ></v-text-field>
          </v-col>

          <v-col
            md="3"
          >
            <v-file-input
              counter
              multiple
              label="Importar nota"
            ></v-file-input>
          </v-col>

          <v-col
            md="3"
          >
            <v-text-field
              label="Prioridade (select with color)"
            ></v-text-field>
          </v-col>
        </v-row>

        <v-row>
          titulo produto
          <v-col
            md="3"
          >
            <v-text-field
              label="produtos"
            ></v-text-field>
          </v-col>
          
          <v-col
            md="3"
          >
            <v-text-field
              label="quantidade"
            ></v-text-field>
          </v-col>

          <v-col
            md="3"
          >
            <v-text-field
              label="Desc"
            ></v-text-field>
          </v-col>

          <v-col
            md="3"
          >
            <v-text-field
              label="valor"
            ></v-text-field>
          </v-col>
          <v-col
            md="3"
          >
            <v-text-field
              label="Observação"
            ></v-text-field>
          </v-col>

          
          <v-col
            md="3"
          >
            <v-text-field
              label="Sugestão(link do produto)"
            ></v-text-field>
          </v-col>
        </v-row>

        <v-row>
          titulo pagamento
          <v-col
            md="3"
          >
            <v-text-field
              label="pagamento"
            ></v-text-field>
          </v-col>
          
          
        </v-row>
      </v-container>
    </v-form>

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
    }),

    methods:{

    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
  