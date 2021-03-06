# Deno Spotify

Access the Spotify API from a Deno CLI app. Uses the [Authorization Code Flow with Proof Key for Code Exchange (PKCE)][1]:

> The authorization code flow with PKCE is the best option for mobile and desktop applications where it is unsafe to store your client secret. It provides your app with an access token that can be refreshed. For further information about this flow, see [IETF RFC-7636][2].

## Usage

A test application is provided:

```shell
> deno run --allow-net https://raw.githubusercontent.com/DavidJones418/deno-spotify/main/spotify_pkce_client_test.ts
Continue authentication at http://localhost:49918
Access token is valid
Current user: {
  ...
}
Current user with refreshed token: {
  ...
}
Continue authentication at http://localhost:49918
Current user with scoped token: {
  ...
}
```

## [MIT License](LICENSE)

[1]: https://developer.spotify.com/documentation/general/guides/authorization-guide/#authorization-code-flow-with-proof-key-for-code-exchange-pkce
[2]: https://tools.ietf.org/html/rfc7636
