<template>
  <article class="block__two">
    <h2 class="two__header">Lorem, ipsum dolor.</h2>
    <div class="text__container">
      <p class="two__text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia, veritatis ad? Facilis nesciunt
        blanditiis tenetur esse? Voluptatem, corrupti sint quia provident recusandae odio culpa voluptate nulla. Ducimus
        repellat aliquid totam!
      </p>
      <p class="two__text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea illum quisquam cum! Similique
        inventore blanditiis cupiditate ipsam. Alias, ut libero laboriosam obcaecati optio ad aliquam molestiae
        praesentium
        exercitationem, quos iusto earum sequi eum autem nulla et perspiciatis quam adipisci? Eius quam autem adipisci
        sit!
        In aliquid tempora quidem tempore atque?
      </p>
      <p class="two__text">
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Fugiat, nihil. Incidunt adipisci nam aperiam quis,
        voluptatem ratione ex aut dolor.
      </p>
    </div>
  </article>
</template>

<script>
export default {
  name: 'article-two'
}
</script>

<style>
.block__two {
  background-image: url('../assets/two__bg.webp');
  background-repeat: no-repeat;
  background-position: 100% 50%;
  background-size: contain;
}

.text__container {
  display: flex;
  flex-direction: column;
  row-gap: 20px;
  max-width: 600px;
  padding: 20px 0;
}

@media(max-width: 1270px) {
  .text__container {
    max-width: 360px;
  }
}

@media(max-width: 945px) {
  .block__two {
    background-position: 50% 100%;
    background-size: calc(50%);
  }

  .text__container {
    max-width: 600px;
    padding-bottom: 200px;
  }
}

@media(max-width: 648px) {
  .text__container {
    padding-bottom: 180px;
  }
}

@media(max-width: 480px) {
  .text__container {
    padding-bottom: 150px;
  }
}

@media(max-width:380px) {
  .block__two {
    background-size: calc(70%);
  }
}
</style>