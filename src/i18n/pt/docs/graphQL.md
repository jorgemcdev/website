# GraphQL

_Extensões suportadas: `gql`, `graphql`_

Podemos importar diretamente um ficheiro GraphQL:

```graphql
# schema.graphql
type Query { hello: String }
```

```js
import schema from './schema.graphql'
```

`schema` é agora um Documento GraphQL

Podemos também utilizar imports:

```graphql
# Foo.graphql
type Foo { bar: String }
```

```graphql
# schema.graphql

# import "./Foo.graphql"

type Query { foo: Foo }
```
