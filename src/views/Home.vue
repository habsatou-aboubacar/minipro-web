<template>
  <div class="home">
    <entete> 
    </entete>
    <corps></corps>
      
    <foot></foot>
  </div>
</template>

<script>
// @ is an alias to /src
import entete from '@/components/Header.vue'
import foot from "@/components/footer.vue"
import corps from "@/components/corp.vue"



export default {
  name: 'Home',
  components: {
    entete,
    foot,
    corps,
    
  
  }
}
</script>
