# Angular (4.x) Spotify Player - Tutorial source code



![Output Preview](spotify-preview-ani.gif "Output Preview")

## Videos (italian only)

You can watch this [YouTube playlist](https://www.youtube.com/playlist?list=PLUioGv_6G9YJ7nH0T43snvKLXc00FAuH1) to see how I wrote this example

> #### UPDATE: Spotify has now closed all its public API. <br>  Now we need to get and inject a token to every XHR request. So I have updated `SpotifyAPIService` in order to work. 


## Development server

1. Download the [Allow-Control-Allow-Origin:*](https://chrome.google.com/webstore/detail/allow-control-allow-origi/nlfbmbojpeacfghkpbjhddihlkkiljbi/related?hl=en) Chrome Extension to avoid CORS issues

2. Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

3. You must [register your own Spotify Application](https://developer.spotify.com/web-api/authorization-guide/) and replace `client_id` and `client_secret` in `SpotifyAPIService`

```typescript
export class SpotifyAPIService {
  client_id = "[YOUR OWN CLIENT ID]";
  client_secret = "[YOUR OWN SECRET KEY]";
  //...
}
```

## Info

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.0.0.
