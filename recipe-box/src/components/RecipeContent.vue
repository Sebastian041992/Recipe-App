<template>
  <div>
    <div class="card text-white bg-dark mb-3 recipe-direction">
      <div class="card-header text-left">Recipe Name</div>
      <div class="card-body">
        <h5 class="card-title">Dark card title</h5>
        <p class="card-text">
          Some quick example text to build on the card title and make up the
          bulk of the card's content.
        </p>
      </div>
      <div class="card-footer d-flex justify-content-around">
        <button type="button" class="btn btn-outline-light">Add Recipe</button>
        <button type="button" class="btn btn-outline-light">Edit Recipe</button>
        <button type="button" class="btn btn-outline-light">
          Delete Recipe
        </button>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "RecipeContent",
};
</script>
<style scoped>
.recipe-direction {
  width: 60%;
  height: 50vh;
  margin: auto;
  border-radius: 15px;
}
</style>
