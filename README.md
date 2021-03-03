# grpc-test-wishlist-golang

Ejemplo sobre protobuf &amp; golang

#GRPC

=> tecnología para comunicar tanto cliente como servidor. RPC (Remote procedure call) , desencadena una acción. No sabemos cuál va a ser esa acción.

=> Viene de la mano de Google, introdujo los PB (Protocol buffer), que son el idioma de comunicación entre cliente y el servidor para comunicarse


### Qué es?

- IDL (Interface Description Language) => la forma en que se van a comunicar el Cliente y el Servidor
- Multilanguage => Puedo usar protocol buffer con muchos lenguajes (Golang, Java, C#, PHP, Python, etc)
- Serialización optimizada (más rapido que xml, JSON). PB trabaja con estructura de datos compilada. Vamos a necesitar un archivo .proto el que nos va a decir cuáles van a ser nuestras interfaces. (describo las interfaces con los archivos que van a compilarse)
- Less error prone => mucho menor el margen de error.
- Con PB podemos mantener el versionado de manera programática dentro de nuestros archivos .proto . Facilita a tener menos errores a la hora de programar

### Qué necesitamos?

- Archivo .proto
- Compilador Protobuffer => https://grpc.io/blog/installation/https://grpc.io/blog/installation/

### Documentación

- https://developers.google.com/protocol-buffers/docs/overview#simple

### Comandos

- `protoc --go_out=. --go_opt=paths=source_relative \
- --go-grpc_out=. --go-grpc_opt=paths=source_relative \
- proto/whishlist.proto`
