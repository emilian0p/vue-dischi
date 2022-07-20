<template>
        <div v-if="discs.length > 9" class="p-0 d-flex flex-wrap justify-content-between">
            <SingleAlbum class="bg-card my-2 text-white"
            v-for="(disc,index) in discs" :key='index'
            :disc=disc />
        </div>

</template>

<script>
    import axios from 'axios';
    import SingleAlbum from './SingleAlbum';
    export default {
        data: function(){
            return{
                discs:[]
            }
            
        },
        
        components:{
            SingleAlbum,
        },
        
        methods:{
            
            getCards(){
                axios.get('https://flynn.boolean.careers/exercises/api/array/music')
                .then((result)=>{
                    this.discs = result.data.response;
                });
            }   
        },
        created(){
            this.getCards();
        }
    }
</script>

<style lang="scss">
.bg-card{
    background-color:#2e3a46;
    width: calc(100% / 5 - 30px);
}
</style>