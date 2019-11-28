<template>
  <section class="recipes">
    <Recipe
      thumbnail="http://1.bp.blogspot.com/-98KPgn-NLk4/VN4YP3b1o0I/AAAAAAAACUM/Dvw6qUQeAuk/s1600/14251-Skewers%2BOn%2BA%2BPlate%2BFast%2BFood%2BHD%2BWallpaperz.jpg"
      title="Heaveness"
      id="1"
      previewText="You know you want it"
    ></Recipe>
    <Recipe
      thumbnail="https://i.pinimg.com/originals/7b/57/cb/7b57cbf75d820e2c968cc5b6bda2849d.jpg"
      title="Delicious"
      id="2"
      previewText="Enjoy life inside life"
    ></Recipe>
  </section>
</template>

<script>
import Recipe from "@/components/Recipe";

export default {
  components: {
    Recipe
  }
};
</script>
<style scoped>
.recipes {
  display: flex;
  flex-flow: column;
  flex-flow: row wrap;
  justify-content: center;
  align-items: center;
}
</style>