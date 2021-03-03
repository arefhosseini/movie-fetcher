# movie-fetcher
Simple movie fetcher app via flutter.

## Features

### Authenticate
First of all user should sign in to the app and get the authorization token & save it to **database**.
If user is authenticated, we proceed to home page, otherwise show the sign in page.

### Fetch movie
we have a search bar in top of the page with **Search here** message. 

If user type something & click the **Search button**, the app fetch movie data from server.
If user scroll down and reach to bottom page, fetch other movie list (we call **Pagination**).
If server get error or something has wrong, show the propper message.

### Movie item
The movie items component should contain poster, name & year like the above:

![Movie Item](https://user-images.githubusercontent.com/11308483/109769634-ba7c6400-7c0f-11eb-80ec-001107719148.png)


**Note**: The movie API key is static and no need to change.

### User Info
we have another page beside of fetch movie that we call User Info page.

In this page, show authentication info such as access token, name, nickname & sub id.
There is no need to show them as UI component, it's enough to show it as text.
**Note**: There should be **Sign out** button to back to Sign in page.

### Sign out expireation
Access token has 24h expiration time, and if it uses to user info API, it gets error.

so we should sign out user automatically after 24h and redirect him to Sign in page.

## APIs
You can access APIs in a **Postman collection** by [this link](http://google.com)
