<template>
        <div class="jumbotron">
            <h1 class="display-3">{{randomDamage}}</h1>
            <p class="lead">{{randomDamage}}</p>
            <hr class="my-2">
            <p>More info</p>
            <p class="lead">
                <a class="btn btn-primary btn-lg" href="" role="button"></a>
            </p>
            <h3 v-if="seen">Now you see me</h3>
  

        </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  randomDamage: function (min, max) {
    return Math.max(Math.floor(Math.random() * max) + 1, min);
  },
};
</script>