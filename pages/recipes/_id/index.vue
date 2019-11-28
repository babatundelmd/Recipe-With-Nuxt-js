<template>
  <section class="single-recipe">
    <h1>{{recipe.title}}</h1>
    <div class="recipe-image">
      <img :src="recipe.thumbnail" :alt="recipe.title" />
    </div>
    <p>{{recipe.descriptionText}}</p>
  </section>
</template>

<style scoped>
.single-recipe {
  display: flex;
  flex-flow: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding: 30px;
}

.recipe-image {
  width: 100%;
}
</style>

<script>
export default {
  asyncData(context) {
    return new Promise((resolve, reject) => {
      setTimeout(() => {
        resolve({
          recipe: [
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
          ].find(el => el.id === context.params.id)
        });
      }, 1500);
    });
  }
};
</script>
