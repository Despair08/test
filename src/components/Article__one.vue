<template>
  <article class="block__one">
    <figure class="card">
      <img src="../assets/article_img.webp" alt="first" class="card__img">
      <figcaption class="card__descr">Lorem ipsum dolor sit amet.Lorem ipsum dolor sit amet.Lorem ipsum dolor sit
        amet.</figcaption>
    </figure>
    <figure class="card">
      <img src="../assets/article_img2.webp" alt="second" class="card__img">
      <figcaption class="card__descr">Lorem ipsum dolor sit amet.Lorem ipsum dolor sit amet.Lorem ipsum dolor sit
        amet.Lorem ipsum dolor sit amet.</figcaption>
    </figure>
    <figure class="card">
      <img src="../assets/article_img3.webp" alt="third" class="card__img">
      <figcaption class="card__descr">Lorem ipsum dolor sit amet.Lorem ipsum dolor sit amet.</figcaption>
    </figure>
    <figure class="card">
      <img src="../assets/article_img4.webp" alt="fourth" class="card__img">
      <figcaption class="card__descr">Lorem ipsum dolor sit amet.</figcaption>
    </figure>
  </article>
</template>

<script>
export default {
  name: 'article-one'
}
</script>

<style>
.block__one {
  display: grid;
  justify-content: center;
  grid-template-columns: repeat(4, 290px);
  gap: 20px;
}

@media(max-width: 1270px) {
  .block__one {
    grid-template-columns: repeat(3, 290px);
  }
}

@media(max-width: 945px) {
  .block__one {
    grid-template-columns: repeat(2, 290px);
  }

}

@media(max-width: 648px) {
  .block__one {
    grid-template-columns: repeat(1, 290px);
  }
}

.card {
  display: flex;
  flex-direction: column;
  row-gap: 10px;
}

.card__img {
  width: 290px;
  height: 200px;
  object-fit: cover;
}
</style>