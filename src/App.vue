<template>
  <div id="app">
    <SandBox />

<body>
	<form>
        <p style="font-size:40px">Pollarizer</p>
        <p style="font-size:15px">Question of the day:</p>
        How many people are needed to change a lamp?<br><br>

    <div>
        <input type="radio" id="1" name="option" value="A"
               checked>
        <label for="huey">1</label>
      </div>
      
      <div>
        <input type="radio" id="2" name="option" value="B">
        <label for="dewey">5</label>
      </div>
      
      <div>
        <input type="radio" id="3" name="option" value="C">
        <label for="louie">0</label>
      </div>

      <div>
        <button type="submit">Submit</button>
      </div>

    </form>

    <pre id="log">
    </pre>

</body>
    
  </div>
</template>

<script>
import SandBox from './components/SandBox.vue'

export default {
  name: 'App',
  components: {
    SandBox
  }
}

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
