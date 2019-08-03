<template>
  <div class="bar-area">
      <div class="bar-container">
          <input type="text" placeholder="Eggs" autofocus v-model="message">
      </div>
  </div>
</template>

<script>
    export default {
        name: 'AddBar',
        computed: {
            message: {
                get () {
                    return this.$store.state.inputText;
                },
                set (value) {
                    this.$store.commit('changeInputText', value)
                }
            }
        }
    }
</script>

<style scoped>
    .bar-area {
        width: 100%;
        display: block;
        height: 400px;
        background-color: lightsteelblue;
        padding: 170px 0px;
        box-sizing: border-box; 
    }

    input {
        width: 500px;
        height: 60px;
        box-sizing: border-box;
        border: 0px;
        font-size: 23px;
        padding: 0px 40px;
        border-radius: 50px;
    }

    input:focus {
        outline: none;
    }
</style>
