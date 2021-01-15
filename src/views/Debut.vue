<template>
    <div class="debut">
        <entete></entete>
        <deb></deb>
        <foot></foot>

    </div>
</template>
<script>
import entete from '@/components/Header.vue'
import foot from "@/components/footer.vue"
import deb from "@/components/debut.vue"
export default {
    name:"debut",
    components:{
    entete,
    deb,
    foot,
    }
    
}
</script>