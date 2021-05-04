# 1 About
This is all about, We love ice cream! Tell us what the top five ice cream shops in Alpharetta are and why.

# 2. Demo

# 3. Screenshots
The application uses real data by leveraging the [Yelp Fusion API](https://www.yelp.com/developers/documentation/v3).

## 3.1. Home
![Yelp Home](images/step1.PNG)

## 3.2. Search for Ice cream shop / restaurants
![Yelp Search](images/Step2.PNG)

# 4. Caveats
* This app uses the [CORS Anywhere](https://github.com/Rob--W/cors-anywhere/#documentation) because the [Yelp Fusion REST API](https://www.yelp.com/developers/documentation/v3) is meant for server to server communication and does not support [CORS])

# 5. How to run this Application
1. go over to the [Yelp Fusion API documentation](https://www.yelp.com/developers/documentation/v3)
2. Click on `Create App` and sign in if you haven't done so already
3. Once you have signed in, click on the `Get Started` button. If you already have an app, then you will already see the API key
4. Fill out the form for [creating a new app](https://www.yelp.com/developers/v3/manage_app)
5. Copy the generated `API key`. This is a [bearer token] that must be put inside the header of each request
6. Navigate to the `src/hooks/yelp-api/config.js` file and assign the `BEARER_TOKEN` variable the following content
   ```
   const BEARER_TOKEN = '<your-token-here>'
   ```
7. Install the dependencies by running `npm install` or `yarn install`
8. Run the app with `npm start` or `yarn start`
