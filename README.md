# gimkit-flooder.js
npm i gimkit-flooder-js

# Example

```js
const Gimkit = require('gimkit-flooder.js');

const options = {
    pin:240981,
    name:'Bot',
    amount:200
};

const flood = ({ pin, name, amount }) => {
    const client = new Gimkit(pin);
    for(i=0;i<amount;i++){
        client.join(name);
    };
};

flood(options);
```
