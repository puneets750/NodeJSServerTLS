# NodeJSServerTLS
Run your own HTTPS server

Generate your own key.

openssl genrsa -out key.pem

openssl req -new -key key.pem -out csr.pem

openssl x509 -req -days 9999 -in csr.pem -signkey key.pem -out cert.pem


run the server as node server.js

go to browser and type https://localhost:8000/


