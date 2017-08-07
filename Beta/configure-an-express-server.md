# configure-an-express-server
https://www.codewars.com/kata/configure-an-express-server/


```
const solution = () => {
  const express = require('express');
  const app = express();

  app.listen(process.env.PORT, process.env.HOST, () => {
    console.log("Your Express app is up and running! \n");
    console.log( "Listening on port " + process.env.PORT + " and host " + process.env.HOST);
  });
};


```

```
const solution = () => {
  var express = require('express');
  var app = express();

  app.get('/', function (req, res) {
    app.set('port', process.env.PORT);
    app.set('host', process.env.HOST);
});

  app.listen(process.env.PORT, process.env.HOST, function (req, res) {
    app.set('port', process.env.PORT);
    app.set('host', process.env.HOST);
  });
};


```
