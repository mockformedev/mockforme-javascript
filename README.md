# mockforme Integration with Vanilla JavaScript

This repository demonstrates how to integrate `mockforme` with an Vanilla Javascript project to easily mock APIs during development.

MockForMe enables quick API simulation, simplifying frontend testing and rapid prototyping.

This example shows how to use mockforme with plain JavaScript (XMLHttpRequest and fetch) in just a few steps.

## Steps

- Add the mockforme script inside the <head> section.
- Initialize mockforme with your access token.
  > **Note:** Get your access token from https://dashboard.mockforme.com/user/token
- Make API requests using:
  - XMLHttpRequest
  - fetch

## Example
```
<html>
  <head>
    <!-- Step 1: Add MockForMe script -->
    <script src="https://cdn.jsdelivr.net/npm/mockforme@latest/dist/mockforme.client.umd.js"></script>

    <script>
      // Step 2: Initialize MockForMe with your token
      var TOKEN = "ACCESS_TOKEN";
      mockforme(TOKEN).run((mockedApis) => {
        console.log("Mocked APIs:", mockedApis);
      });
    </script>

    <script>
      // Check index.html for function implementation

      function clearText() {}

      function getUserDetailsXhr() {}

      function getUserDetailsFetch() {}
    </script>
  </head>
  <body>
    <button onClick="getUserDetailsXhr()">Get User Details (XHR)</button>
    <button onClick="getUserDetailsFetch()">Get User Details (Fetch)</button>

    <pre id="output"></pre>
  </body>
</html>
```

### Tags
- mockforme integration with vanilla javascript
- mockforme javascript example
- mockforme integration with pure javascript
- mock api testing with mockforme
- how to mock api in javascript
- mockforme quick start
- mockforme xhr fetch example
- mock api integration guide
- mock api without backend
- mockapi using mockforme