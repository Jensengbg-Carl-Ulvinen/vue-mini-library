<template>
  <section>
      <BooksList v-bind:books="books" />
  </section>
</template>

<script>
import books from './assets/childrensbooks.json';
import BooksList from './views/books';

export default {
    components: {
        BooksList
    },
    computed: {
        books() {
            return books.books;
        }
    }
}
</script>

<style>

</style>