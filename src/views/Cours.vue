<template>
<div class="Cours">
    <h1>this is a cours</h1>
    <foot></foot>
    <Cours></Cours>
    </div>

</template>
<script>
import foot from "@/components/footer.vue"
import Cours from "@/components/Cour.vue"

export default {
    name:'Cours',
    components:{
        foot,
        Cours,
    }

}
</script>