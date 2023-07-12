<template>
    <h1>A single user with ID: {{ $route.params.id  ? $route.params.id  : "Unknown" }}</h1>

</template>

<script >

// export default {
//   mounted() {
//     // this.validate(this.$route.params.id || "Unknown");
//     this.validate(this.$route);
//   },
//   methods: {
//     validate(data) {
//       console.log(data);
//     // can use this route only if the answer is true
//       return /^\d+$/.test(data.params.id);
//     }
//   }
// }


export default {

    validate(data) {
      console.log(data);
      return  /^\d+$/.test(data.params.id);
    },
    layout: "users"
}
</script>

<style  scope>

</style>
