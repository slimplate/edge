# edge

These functions enable GitHub authentication and facilitate communication with external APIs while adhering to CORS policies in Vercel projects.

```js
validRedir(redirectUrlString, url) // Checks if a URL matches wildcard patterns in redirectUrlString.
ghcallback(req, res, REDIRECT_URL, GITHUB_CLIENT, GITHUB_SECRET) // Handles GitHub OAuth callback, exchanges code for token, and redirects to authorized URL.
ghlogin(req, res, REDIRECT_URL, GITHUB_CLIENT) // Initiates GitHub login flow and redirects to GitHub OAuth authorization endpoint.
cors(req, res) // Acts as a CORS proxy for external API requests, handling headers and forwarding the request.
```