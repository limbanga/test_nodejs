# Learn Expressjs

limbanga is learning how to use express in ubuntu :)

Here is his note

## Install node

First step, I download nodejs from node homepage in *.tar.xz format.
I have unziped this file using bash scripts

```bash
tar -xfv <nodejs_file.tar.xz>
```

I recieved a folder contain nodejs code.

I have moved it into my /home/<username> folder for management.
Then I add bin folder's path to ~/.bashrc so that I can access nodejs code though my terminal.

For example:

```bash
export PATH=$PATH:/home/lim/node-v20.17.0-linux-x64/bin
```

It can be different rely on where your store the folder

Now restart your terminal and start coding

```bash
source ~/.bashsrc
```

If your installation is succeed, this code should print node version

```bash
node -v
```


## Initialize node project

npm init enter enter enter! to init a nodejs project :)

```bash
npm init
```

You'll see package.json file containing project information.

## Install Express

To install express

```bash
npm install express
```

Let's check the change in package.json
You'll see express in dependencies

## Create first app and run

Create index.js file and paste this code

```js
const express = require('express');
const app = express();
const port = 3000;

app.get('/', (req, res) => {
  res.send('Hello World!');
});

app.listen(port, () => {
  console.log(`Example app listening at http://localhost:${port}`);
});
```

Run this code!

```bash
node index.js
```

Open your browse and test this url localhost:3000
