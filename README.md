# ESNext Boilerplate

```bash
# clone this repo
git clone https://github.com/reggi/esnext-boilerplate.git
# cd into the downloaded repo
cd esnext-boilerplate
# install babel (locally)
npm install
# use this to watch the src dir
npm run babel-node-watch
# or just run babel with
npm run babel-node
```

# Async / Await

Below is an example using `async` and `await`. You have to make sure the dependency `"babel-polyfill"` is included.

```js
import "babel-polyfill"

async function five() {
  return 5
}

async function helloWorld() {
  var numb = await five()
  console.log(numb)
}

helloWorld() // logs `5`
```
