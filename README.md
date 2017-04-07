# Lazy,

![](https://cagatay.js.org/lazy.png)

## AI telegram chat bot.

<p>Lazy allows you create awesome chat bot with no longer know ai!</p>
<p>Just teach lazy 4 your phase case!</p>
<p>Let him answer you instead!</p>

You can try in telegram already: Lets chat with @LazyAIBot, my Turkish friends already teached somethings like as greetings.
If you want host on your own, go ahead do this!
[Create telegram bot.](https://core.telegram.org/bots#6-botfather)

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/cagataycali/lazy)

## Programmatic Usage

```bash
# Or npm install --save lazy.ai
$> yarn add lazy.ai
```

```javascript
var Lazy = require('lazy.ai');

async function start() {
  var lazy = new Lazy();
  // Learn ..
  console.log(await lazy.learn({phrase: 'hello', category: 'greetings'}));
  console.log(await lazy.learn({phrase: 'hi', category: 'greetings'}));
  console.log(await lazy.learn({phrase: 'Hello there!', category: 'greetings'}));
  // Result ..
  console.log(await lazy.query({phrase: "hello dude!"}));
  // Helpers..
  console.log(await lazy.addResponse({category: 'greetings', response: 'Hi there!'}));
  console.log(await lazy.getResponses({category: 'greetings'}));
  console.log(await lazy.getCategories());
}
// Dont forget start your function :)
start();
```

[![See in action](https://asciinema.org/a/9fnkllfe8pkddzddkem7iiq8t.png)](https://asciinema.org/a/9fnkllfe8pkddzddkem7iiq8t)

## Telegram Bot Usage

<details>

### Learn something..

```
/learn hi - greeting
```

### Add some greeting message..

```
/add greeting - Hello there!
/add greeting - Hello buddy!
```

### Show categories

```
/categories
```

### Show responses

```
/responses greeting
```

### Just quiet

```
/quiet
```

### Save trained output

```
/save
```

### Load trained output

```
/load
```
</details>

## License

MIT © [cagataycali](https://cagatay.me)
