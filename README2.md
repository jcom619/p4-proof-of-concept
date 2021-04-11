# <center >


| <center>☀️ weather-UI ☀️
|-
| <center>dynamic UI that changes according to local weather and time zone changes

<img src="https://media2.giphy.com/media/k8aCl2VvSeBlRvL7Yf/giphy.gif?cid=5e214886936f38bc795d75080a46c7c1c0ce7bdc0f88320b&rid=giphy.gif&ct=g">

TECH IMPLIMENTATIONS:

- SASS (css pre-compiler)
- M.E.R.N. (needs no introduction)
- open Weather **_API_**

  <https://rapidapi.com/community/api/open-weather-map?endpoint=53aa6041e4b00287471a2b62>

- Customize Bootstrap with the theme kit
  How to build your own Bootstrap themes

  <https://hackerthemes.com/kit/>

USERS:

- Anyone, mostly developers and students

COULD BE PROBLEMS:

- implimenting google APIs ( they are surely reliable but difficult as I understand )
- not sure how to pull this one off

TO BE DONE!...

Study - how to impliment the following

<https://hackerthemes.com/kit/> "customize BS variables"

apply some logic to automate classname alternation

**_DONE!..._**

Test -
<https://rapidapi.com/community/api/open-weather-map?endpoint=53aa6041e4b00287471a2b62>

( no personal API key required )

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
