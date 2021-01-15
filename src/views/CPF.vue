<template>
<div class="cpf">
    <entete></entete>
    <br>
    <cpfe></cpfe>
    <br>
     <foot></foot>
</div>  
</template>
<script>
import entete from '@/components/Header.vue'
import foot from "@/components/footer.vue"
import cpfe from '@/components/Cpf.vue'
export default 
{
    name :'cpf',
    components:{
        cpfe,
        foot,
        entete,

    }
    
    
    
}
</script>