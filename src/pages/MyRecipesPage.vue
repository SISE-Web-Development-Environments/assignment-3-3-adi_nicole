<template>
  <div class="container">
    
    <h1 class="title">My Recipes</h1>
    <div>
      <RecipePreviewList title="" pageType="myrecipes"  :recipesList="recipes" class="MyRecipes center" />
    </div>
  </div>
</template>

<script>
import RecipePreviewList from "../components/RecipePreviewList";
export default {
  components: {
    RecipePreviewList
  },
  data(){
    return{
      recipes: []
    };
  },
};
</script>

<style lang="scss" scoped>
.MyRecipes {
  margin: 10px 0 10px;
  width: 600px;
  height: 800px;
}
.title{
    background: url("https://previews.123rf.com/images/romastudio/romastudio1603/romastudio160300234/54088727-healthy-food-background-and-copy-space-studio-photo-of-different-fruits-and-vegetables-on-white-wood.jpg");
    color: white;
    -webkit-text-stroke-width: 1px;
    -webkit-text-stroke-color: black;
    text-align: center;
    font-family:"Trebuchet MS", Helvetica, sans-serif;
    font-size: 43px;
    font-weight: bold;
}

</style>
