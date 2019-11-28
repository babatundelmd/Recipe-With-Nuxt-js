<template>
  <section class="recipes">
    <article class="recipe">
      <div
        class="thumbnail"
        style="background-image: url('http://1.bp.blogspot.com/-98KPgn-NLk4/VN4YP3b1o0I/AAAAAAAACUM/Dvw6qUQeAuk/s1600/14251-Skewers%2BOn%2BA%2BPlate%2BFast%2BFood%2BHD%2BWallpaperz.jpg')"
      ></div>
      <div>
        <h1>Title</h1>
        <p>Some nice preview text</p>
      </div>
    </article>

    <article class="recipe">
      <div
        class="thumbnail"
        style="background-image: url('https://i.pinimg.com/originals/7b/57/cb/7b57cbf75d820e2c968cc5b6bda2849d.jpg')"
      ></div>
      <div>
        <h1>Title</h1>
        <p>Some nice preview text</p>
      </div>
    </article>
  </section>
</template>


<style scoped>
.recipes {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-items: center;
}

.recipe {
  box-sizing: border-box;
  width: 280px;
  padding: 8px;
  border: 1px solid #ccc;
  box-shadow: 0 2px 2px #eee;
  margin: 10px;
  border: none;
}

.thumbnail {
  background-position: center;
  background-size: cover;
  width: 100%;
  height: 200px;
}
</style>