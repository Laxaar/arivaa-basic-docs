# Analytics

In Arivaa Firebase, We have used Segment Analytics, one of the leading platform in performing in-app analytics using events and screen triggers.

**Architecture**

We have created a helper \(src/utils/analytics.js\) for you to manage to manage the analytics flow.

Configuration is done under src/config/analytics.js. \(You will need to change the API Key here\).

**Guide**

1. Create an account on segment [portal](https://app.segment.com).
2. Create 2 sources for ios and android.
3. Go to each source and then to settings/API Keys and copy the write key for ios and android.
4. Update the api keys in src/config/analytics.js
5. You can start firing events in the application using trackEvent and recordScreenTransition methods present in src/config/analytics.js.
6. View the events and screen transitions in the debugger.
7. Optional - In order to route these analytics to destinations like google analytics, you can create and configure destinations also in segment portal. No setup required on application end.

**Detailed Reference Docs :**

1. {% embed data="{\"url\":\"https://docs.expo.io/versions/v26.0.0/sdk/segment\",\"type\":\"link\",\"title\":\"Segment - Expo Documentation\",\"icon\":{\"type\":\"icon\",\"url\":\"https://docs.expo.io/static/images/favicon.ico\",\"width\":32,\"height\":32,\"aspectRatio\":1}}" %}
2. {% embed data="{\"url\":\"https://segment.com/docs/\",\"type\":\"link\",\"title\":\"Documentation Documentation - Segment\",\"description\":\"The technical documentation for Segment.\",\"icon\":{\"type\":\"icon\",\"url\":\"https://segment.com/build/public/public/images/touch-icon.png\",\"width\":192,\"height\":192,\"aspectRatio\":1},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://segment.com/build/public/public/images/open-graph.png\",\"width\":1200,\"height\":1200,\"aspectRatio\":1}}" %}





