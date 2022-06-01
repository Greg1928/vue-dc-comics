<template>
  <main>
      <div class="container">
          <p>-->content goes here--</p>
      </div>
  </main>
</template>

<script>
export default {
    name: "BaseMain",
}
</script>

<style lang="scss" scoped>
main{
    background-color: var(--secondary-color);

    & .container p{
        padding: 4.375rem 0;
        color: white;
        font-size: 2.5rem;
    }
}
</style>