<template>
    <div>
      <button @click="plus">+</button>
      <button @click="minus">-</button>
      <p><span>{{lal}}</span></p>
    </div>
</template>

<script>
    export default {
      props: ["lal"],
        data() {
          return {
            lal: 0
          }
        },
      methods: {
          plus() {
            this.$emit("plus");
          },
        minus() {
          this.$emit("minus");
          }
      }
    }
</script>
