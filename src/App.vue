<template>
  <div id="app">
    <main>
      <div class="search-box">
        <input 
        type="text" 
        class="search-bar" 
        placeholder="Search...">
      </div>

      <div class="weather-wrap">
        <div class="location-box">
          <div class="location">Johor, Malaysia</div>
          <div class="date">Saturday 9 July 2022</div>
        </div>

        <div class="weather-box">
          <div class="temp">25°C</div>
          <div class="weather">Night</div>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  components: {

  },
  data() {
    return{
      api_key: '5f6a236e939b8ab1a70b57ab330b06ce',
    }
  },
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app{
  background-image: url('./assets/cold-bg.jpg');
  background-size: cover;
  background-position: bottom;
  transition: 0.4s;
}

main {
  min-height: 100vh;
  padding: 25px;
  background-image: linear-gradient(to bottom, rgba(0,0,0,0.25), rgba(0,0,0,0.75));
}

.search-box {
  width: 100%;
  margin-bottom: 30px;
}

.search-box .search-bar{
  display: block;
  width: 100%;
  padding: 15px;

  color: #313131;
  font-size: 20px;

  appearance: none;
  border: none;
  outline: none;
  background: none;

  background-color: rgba(255,255,255,0.5);
  border-radius: 0px 16px;
  box-shadow: 0px 0px 16px rgba(0,0,0,0.25);
  transition: 0.4s;
}

.search-box .search-bar:focus {
  background-color: rgba(255,255,255,0.75);
  box-shadow: 0px 0px 16px rgba(0,0,0,0.25);
  border-radius: 0px 16px;
}

.location-box .location{
  color: #FFF;
  font-size: 32px;
  font-weight: 500;
  text-align: center;
  text-shadow: 1px 3px rgba(0,0,0,0.25);
}

.location-box .date{
  color: #FFF;
  font-size: 32px;
  font-weight: 500;
  text-align: center;
  text-shadow: 1px 3px rgba(0,0,0,0.25);
}

.weather-box{
  text-align: center;
}

.weather-box .temp{
  display: inline-block;
  padding: 10px;
  color: #FFF;
  font-size: 100px;
  font-weight: 700;
  background-color: rgba(255,255,255,0.25);
  border-radius: 16px;
  margin: 30px 0px;
  text-shadow: 3px 6px rgba(0,0,0,0.25);
}

.weather-box .weather{
  color: #FFF;
  font-size: 48px;
  font-weight: 700;
  font-style: italic;
  text-shadow: 3px 6px rgba(0,0,0,0.25);
}
</style>
