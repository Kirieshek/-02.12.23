<template>
    <div>
    {{ text }} <br>
    <br>
    <button @click="change">Изменить содержимое текста</button><br>
    <button @click="say('Привет')">Изменить содержимое текст на "Привет"</button><br>
    <button @click="say('Пока')">Изменить содержимое текста на "Пока"</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: 'xxx'
    }
  },
  methods: {
    change() {
      this.text = 'yyy' 
    },
    say(text) {
      this.text = text 
    }
  }
}
</script>

<style>
  
</style>
