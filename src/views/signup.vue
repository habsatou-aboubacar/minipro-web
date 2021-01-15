<template>
<div class="signup">
  <entete></entete>
  <br>
    <signe></signe>
    <foot></foot>
</div>
    
</template>
<script>
import entete from "@/components/Header.vue"
import signe from "@/components/inscription.vue"
import foot from "@/components/footer.vue"
export default {
    name: 'sign',
  components: {
    entete,
    signe,
    foot,
  }
}
</script>