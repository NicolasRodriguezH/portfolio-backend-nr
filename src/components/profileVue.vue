<template>
    
    <b-container>
     <b-card class="mt-5 rounded shadow-lg" style="background-color: rgba(0, 0, 0, 0.5);">
          <span class="font-weight-bold" style="color: #f8f9fa; opacity: 0.8;">Personal Profile</span> <br>
          <hr>
          <p class="font-italic" style="color: #f8f9fa; opacity: 0.8;">
            I am a person who believes in the power of teamwork, in growing and learning more every day, an art lover and who does not give up on his ambitions.
            </p>
     </b-card>

     <!-- Mirar si dejar esta seccion o no -->
      <b-card class="mt-1 rounded shadow-sm" style="background-color: rgba(0, 0, 0, 0.5);">
          <span class="font-weight-bold" style="color: #f8f9fa; opacity: 0.8;">Enhancers</span> <br>
          <hr>
          <!-- <b-badge>
            Backend-developer
          </b-badge> -->
          <br>   
         <b-badge variant="dark">
            Game Developer
         </b-badge>
         <br>
         <b-badge>
            Generalist             
         </b-badge>
         <br>
         <b-badge variant="dark">
            A real art developer
         </b-badge>
     </b-card>
 </b-container>
  

</template>

<script>
export default {
    name: 'profileVue'
}
</script>