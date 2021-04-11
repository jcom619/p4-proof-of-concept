

 | <center><h1> ☀️ Weather-UI ☀️ </h1> <br> <br>dynamic UI that changes according to local weather and time zone changes<hr><br>*****************************************************<br><img src="https://media2.giphy.com/media/k8aCl2VvSeBlRvL7Yf/giphy.gif?cid=5e214886936f38bc795d75080a46c7c1c0ce7bdc0f88320b&rid=giphy.gif&ct=g"><br><br>***************************************************** <hr> <h3>TECH: </h3> <br> <br><br>SASS (css pre-compiler) <br><br> M.E.R.N.<br>(needs no introduction) <br><br>[**_OpenWeather API_**](https://rapidapi.com/community/api/open-weather-map?endpoint=53aa6041e4b00287471a2b62)<br><hr> 🕺 🏌️ 🚶 🤼‍♂️ 🏋️‍♂️ 🤸 🤾 🕴️💃 🕺 🏌️ 🚶 🤼‍♂️ 🏋️‍♂️ 🤸 🤾 🕴️💃 🕴️🕴️ <br> USER STORIES:<br><br>- <br><br>-<br><br>-<br><br>-<br><br> <hr><br>TO BE DONE!...<br><br>- <br><br>-<br><br>-<br><br>-<br><br> <br><br>******************** <br>Study how to impliment the following<br> [for ideas](https://hackerthemes.com/kit/> "customize BS variables")<br><br> apply some logic to automate styles based on API output<br><br>***************************************************** <br><center> **_DONE!..._** <br><br>- <br><br>-<br><br>-<br><br>-<br><br> <br>------------------------------------------------------------------------------------------------------------
 |-


* Test<br>
[open-weather-map](https://rapidapi.com/community/api/open-weather-map?endpoint=53aa6041e4b00287471a2b62)



```js
// sample code

fetch(
  "https://community-open-weather-map.p.rapidapi.com/weather?q=London%2Cuk&lat=0&lon=0&callback=test&id=2172797&lang=null&units=%22metric%22%20or%20%22imperial%22&mode=xml%2C%20html",
  {
    method: "GET",
    headers: {
      "x-rapidapi-key": "d5780d7757msh7c61b742690e076p1596bbjsn7ad45870345d",
      "x-rapidapi-host": "community-open-weather-map.p.rapidapi.com",
    },
  }
)
  .then((response) => {
    console.log(response);
  })
  .catch((err) => {
    console.error(err);
  });
```

result:

```json
test({
  "coord": {
    "lon": -116.5453,
    "lat": 33.8303
  },
  "weather": [
    {
      "id": 800,
      "main": "Clear",
      "description": "clear sky",
      "icon": "01d"
    }
  ],
  "base": "stations",
  "main": {
    "temp": 299.06,
    "feelslike": 297.89,
    "tempmin": 292.59,
    "temp_max": 307.15,
    "pressure": 1013,
    "humidity": 7
  },
  "visibility": 10000,
  "wind": {
    "speed": 2.57,
    "deg": 70
  },
  "clouds": {
    "all": 1
  },
  "dt": 1617995965,
  "sys": {
    "type": 1,
    "id": 5412,
    "country": "US",
    "sunrise": 1617974542,
    "sunset": 1618020748
  },
  "timezone": -25200,
  "id": 5380668,
  "name": "Palm Springs",
  "cod": 200
})
```
