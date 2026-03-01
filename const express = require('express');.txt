const express = require('express');
const app = express();
const path = require('path');

app.use(express.static(path.join(__dirname)));

app.listen(3000, '0.0.0.0', () => {
  console.log('Servidor rodando em http://0.0.0.0:3000');
});