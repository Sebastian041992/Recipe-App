<template>
  <div class="card recipe-card border border-dark bg-dark my-2">
    <table class="table table-hover table-dark w-100 text-left m-0">
      <tbody>
        <tr>
          <td>{{ recipe.title }}</td>
        </tr>
        <tr>
          <td class="p-3">2</td>
        </tr>
        <tr>
          <td class="p-3">3</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>
<script>
export default {
  name: "RecipeTitles",
  props: ["title"],
  data() {
    return {
      recipe: null,
    };
  },
  mounted() {
    fetch("http://localhost:3000/recipe" + this.title)
      .then((res) => res.json())
      .then((data) => (this.recipe = data))
      .catch((err) => console.log(err.message));
  },
};
</script>
<style scoped>
.recipe-card {
  width: 60%;
  height: 20vh;
  margin: auto;
  overflow: auto;
  border-radius: 15px;
}
</style>
