<template>
    <div id='listapr'>
        <div class='row justify-content-center'>
            <div class='col-sm-5' v-for="proizvod in proizvodi" :key="proizvod.id">
                <router-link :to='/detaljiproizvoda/+proizvod.id'> 
                    <Proizvod :pr="proizvod"></Proizvod>
                </router-link> 
            </div> 
        </div>
    </div>
</template>

<script>
import Proizvod from './Proizvod.vue'

export default {
    name: 'ListaProizvoda',
    components:{
        Proizvod
    },
    data(){
        return{
            proizvodi: [
                {
                    id: 1,
                    naziv: 'Pedigree',
                    cena: '1000din',
                    opis: 'Young adult',
                    ocena: 5
                },
                {
                    id: 2,
                    naziv: 'Pedigree',
                    cena: '3000din',
                    opis: 'Adult',
                    ocena: 4
                },
                {
                    id: 3,
                    naziv: 'Meow Mix',
                    cena: '1000din',
                    opis: 'Chicken',
                    ocena: 5
                },
                {
                    id: 4,
                    naziv: 'Meow Mix',
                    cena: '1200din',
                    opis: 'Chicken',
                    ocena: 4
                }
            ]
        }
    }
}
</script>