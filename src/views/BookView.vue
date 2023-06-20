<template>
  <div class="about">
    <h1>WELCOME</h1>
    <BookMenu />
  </div>
</template>

<script>
import BookMenu from '@/components/book.vue';

export default {
  name: 'BookView',
  components: {
    BookMenu
  },
  data() {
    return {
      inputText: "",
      num: 50
    };
  }
};
</script>
