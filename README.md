# Formata
Official [Formata.io](https://formata.io) API client.

## Install
```
$ npm install --save formata
```
or
```
$ yarn add formata
```

## Delivering data
```js
import Formata from 'formata'

const formata = new Formata('YOUR_SK_API_KEY')

formata.deliver(bucketName, {
  name: "John Smith",
  email: "hello@johnsmith.name"
}).then(res => {
  // response.ok
})
.catch(err => {
  //Some error
})
```

## Fetching data
```js
import Formata from 'formata'

const formata = new Formata('YOUR_SK_API_KEY')

formata.deliver(bucketName, {
  limit: 3,
  sort: 'name'
}).then(res => {
  // response.ok
})
.catch(err => {
  //Some error
})
```
