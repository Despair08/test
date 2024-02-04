<template>
  <div class="header__container">
    <button class="header__button" v-on:click="isSeen">
      {{ label }}
    </button>
    <div class="buttons__container" v-if="seen">
      <button class="header__button" v-for="user in users" :key='user.id'>
        {{ user.title }}
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'header-button',
  data: function () {
    return {
      label: 'Push me!',
      seen: false,
      users: [
        {
          id: 1,
          title: 'Админ',
          role: 'admin'
        },
        {
          id: 2,
          title: 'Сотрудник',
          role: 'employee'
        },
        {
          id: 3,
          title: 'Гость',
          role: 'guest'
        }
      ]
    };
  },
  components: {

  },
  methods: {
    isSeen: function () {
      this.seen = !this.seen;
    }
  }
}
</script>

<style>
.header__container {
  display: flex;
  padding: 10px 20px;
  column-gap: 20px;
}

@media(max-width:460px) {
  .header__container {
    flex-direction: column;
    row-gap: 10px;
    align-items: center;
  }
}

.buttons__container {
  display: flex;
  column-gap: 20px;
}

.header__button {
  display: block;
  height: 30px;
  width: 80px;
  border-radius: 5px;
  border: none;
}

.header__button:hover {
  border: 1px solid #000;
  cursor: pointer;
}

.header__button:active {
  transform: translate(0, 1px);
}
</style>