<template>
  <div class="about">
        <entete></entete>

        
    <h1>This is an about page</h1>

   <foot></foot> 
  </div>
</template>
<script>
// @ is an alias to /src
import entete from '@/components/Header.vue'
import foot from "@/components/footer.vue"
export default {
  name: 'about',
  components: {
    entete,
    foot
  }
}
</script>
