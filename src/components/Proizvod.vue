<template>
    <div id='proizvod'>
        <div class='card'>
            <img class='card-img-top' :src="'/img/img'+pr.id+'.png'">
            <div class='card-body'>
                <h4>{{pr.naziv}}</h4>
                <h6>{{pr.cena}}</h6>
                <p>{{pr.opis}}</p>
            </div>
        </div>
    </div>
</template>

<style>
    img{
        width:30%;
    }
</style>

<script>
export default {
    name: 'Proizvod',
    props: [
        'pr'
    ]
}
</script>