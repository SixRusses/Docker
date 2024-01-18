FROM node:14

WORKDIR /usr/src/app

COPY index.html .

EXPOSE 8080

CMD ["node", "-e", "const http = require('http'); const fs = require('fs'); const server = http.createServer((req, res) => { fs.readFile('index.html', 'utf8', (err, data) => { res.writeHead(200, {'Content-Type': 'text/html'}); res.end(data); }); }); server.listen(8080); console.log('Server running on port 8080');"]
