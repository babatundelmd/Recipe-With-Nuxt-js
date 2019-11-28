<template>
  <section class="recipes">
    <Recipe
      v-for="recipe in recipes"
      :key="recipe.id"
      :thumbnail="recipe.thumbnail"
      :title="recipe.title"
      :id="recipe.id"
      :previewText="recipe.previewText"
    ></Recipe>
  </section>
</template>

<script>
import Recipe from "@/components/Recipe";

export default {
  components: {
    Recipe
  },
  asyncData() {
    return new Promise((resolve, reject) => {
      setTimeout(() => {
        resolve({
          recipes: [
            {
              id: "1",
              title: "Heaveness",
              previewText: "You know you want it",
              descriptionText: "This is a really nice meal",
              thumbnail:
                "http://1.bp.blogspot.com/-98KPgn-NLk4/VN4YP3b1o0I/AAAAAAAACUM/Dvw6qUQeAuk/s1600/14251-Skewers%2BOn%2BA%2BPlate%2BFast%2BFood%2BHD%2BWallpaperz.jpg"
            },

            {
              id: "2",
              title: "Delicious",
              previewText: "Awesome Delicacy",
              descriptionText: "Intercontinental Meal",
              thumbnail:
                "https://i.pinimg.com/originals/7b/57/cb/7b57cbf75d820e2c968cc5b6bda2849d.jpg"
            }
          ]
        });
      }, 1500);
    });
  }
};
</script>
<style scoped>
.recipes {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-items: center;
}
</style>