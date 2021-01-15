<template>
<div class="Connecter">

   
    <entete></entete><br>
    <connecte></connecte>
    <br>
     <foot></foot>
</div>  
</template>
<script>
import entete from '@/components/Header.vue'
import foot from "@/components/footer.vue"
import connecte from '@/components/authentifi.vue'
export default 
{
    name :'connecter',
    components:{
        connecte,
        foot,
        entete,

    },
    methods: {

    }
    
    
    
}
</script>