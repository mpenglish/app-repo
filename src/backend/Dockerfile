FROM node:18-alpine
WORKDIR /app
# Return a JSON payload
RUN echo 'const http = require("http"); \
http.createServer((req, res) => { \
  res.writeHead(200, { "Content-Type": "application/json" }); \
  res.end(JSON.stringify({ message: "Hello from the Node.js Backend API! This is a chanage to the backend" })); \
}).listen(8080);' > server.js
EXPOSE 8080
CMD ["node", "server.js"]