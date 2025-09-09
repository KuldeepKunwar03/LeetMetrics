# LeetMetrics
Track your LeetCode progress instantly. This tool fetches and displays key stats from any user profile: the total number of unique questions solved and the total number of submissions made. It's a simple, clean dashboard to monitor your coding consistency and stay motivated.
<br>
<br>
⚙️ How It Works
<br>
<br>
This application is built entirely on the frontend and does not require its own backend. It directly queries LeetCode's public GraphQL endpoint to fetch user data.
<br>
<br>
https://leetcode.com/graphql/
<br>
<br>
To overcome the Cross-Origin Resource Sharing (CORS) policy enforced by browsers (which prevents a web page from making requests to a different domain), this project uses a public CORS proxy.
<br>
<br>
<br>
const proxyUrl = "https://cors-anywhere.herokuapp.com/";
<br>
const targetUrl = "https://leetcode.com/graphql/";
<br>
<br>
The application sends its request to the proxyUrl, which then forwards it to the targetUrl. The proxy adds the necessary CORS headers to the response, allowing the browser to accept it.

