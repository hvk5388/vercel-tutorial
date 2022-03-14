# Learn How APIs Work

API's are confusing. I barely understand them myself, but they are so useful. Outsourcing code can make your life so much easier. API's are very helpful in communicating with other services. Today I'm gong to go through what happens when you request from the [Wikipedia API](https://en.wikipedia.org/w/api.php) with data from a locational API.

# The request

A fetch call is used to send a request to the locational API. This is so the API will help them retrieve data. In this example we fetch the location and IP address of of the user. The request code is shown below. You can see that the data is then saved as variables.

```javascript
return fetch(this.locationEndpoint + userIPData.ip)
  .then((resp) => {
    if (resp.ok) {
      return resp.json();
    }
    return false;
  })
  .then((data) => {
    console.log(data);
    this.lat = data.latitude;
    this.long = data.longitude;
    this.city = data.city;
    this.state = data.region_name;
    console.log(`${this.lat} ${this.long}`);
    return data;
  });
```

# Wikipedia API

The Wikipedia API has many functions but we are using the query function. In this function the action of querying sends us the information that we are looking for. In our code we stored the response from the location in variables. We can use these variables as the search when we call the Wikipedia API.

```javascript
<wikipedia-query search="${this.city}, ${this.state}"></wikipedia-query>
<wikipedia-query search="${this.city}"></wikipedia-query>
<wikipedia-query search="${this.state}"></wikipedia-query>
```

Once these are called in the page the response is displayed as a Wikipedia article if one exists. With the use of these two APIs and very little coding on our part we have a working program that displays an article specific to the user.
