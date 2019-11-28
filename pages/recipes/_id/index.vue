<template>
  <section class="single-recipe">
    <h1>{{$route.params.id}}</h1>
    <div>
      <img src alt />
    </div>
    <p>The recipe desciption</p>
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
}
</style>

<script>
export default {
  // asyncData(context) {
  //   return new Promise((resolve, reject) => {
  //     setTimeout(() => {
  //       resolve({
  //         recipe: [
  //           {
  //             id: "1",
  //             title: "Delicious",
  //             previewText: "Awesome Meal",
  //             descriptionText: "This is a really nice meal",
  //             thumbnail:
  //               "http://1.bp.blogspot.com/-98KPgn-NLk4/VN4YP3b1o0I/AAAAAAAACUM/Dvw6qUQeAuk/s1600/14251-Skewers%2BOn%2BA%2BPlate%2BFast%2BFood%2BHD%2BWallpaperz.jpg"
  //           },
  //           {
  //             id: "2",
  //             title: "Delicious Cuisine",
  //             previewText: "Awesome Delicacy",
  //             descriptionText: "Intercontinental Meal",
  //             thumbnail:
  //               "http://1.bp.blogspot.com/-98KPgn-NLk4/VN4YP3b1o0I/AAAAAAAACUM/Dvw6qUQeAuk/s1600/14251-Skewers%2BOn%2BA%2BPlate%2BFast%2BFood%2BHD%2BWallpaperz.jpg"
  //           }
  //         ]
  //       });
  //     }, 1500);
  //   });
  // }
};
</script>