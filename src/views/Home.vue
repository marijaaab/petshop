<template>
  <div class="home">
    <h1>PetShop Maza</h1>
    <h3>Sve za Vase ljubimce!</h3>
    <button class="btn btn-success" @click="login()">Prijavi se!</button>
    <hr/>
    <br/>
    <ListaProizvoda></ListaProizvoda>
    <modal name='prijavaModal'>
     Hello!
    </modal>
  </div>
</template>

<script>
// @ is an alias to /src
import ListaProizvoda from '../components/ListaProizvoda.vue'

export default {
  name: 'Home',
  components:{
    ListaProizvoda
  },
  methods:{
    login(){
      this.$modal.show('prijavaModal')
    }
  }
}
</script>
