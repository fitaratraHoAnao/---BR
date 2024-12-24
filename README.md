## ABOUT ME

name : ```Ryuko Developer```</br>
age : ```18```</br>
link : [facebook](https://www.facebook.com/ryukodev).</br>
## START UP

```txt
npm install
```
```txt
node index.js
```

## SOURCES

original file : [BotPack](https://replit.com/@YanMaglinte/BotPack?v=1) by ```YanMaglinte```</br>
modified : [ryuko](https://github.com/ryukodeveloper/Ryuko-V4) by ```Ryuko Developer```</br>
fca : [ws3-fca](https://www.npmjs.com/package/ws3-fca) by ```Kenneth Aceberos```

## UPDATES

• added email function, this updates belongs to premium system and box approval system. if the user is requesting for approval the notification will sent from your email address. enter your email address at ``ryuko.json``.</br>
• fixed spam in ban system.</br>
• discover the new feature with ```premium command```, you can enable it by adding a variable named ```premium``` and the value is boolean</br></br>
```premium ussage example```
```js
module.exports.config = {
  name: "example",
  version: "example",
  credits: "example",
  permission: 0,
  description: "example",
  category: "example",
  usages: "example",
  prefix: true,
  premium: true, // this is the example of premium feature ussage
  cooldown: 0,
  dependencies: {
    "": ""
  }
}
```
```txt
UPCOMING UPDATE :
adding aliases for each commands
adding prefix config for each bots
adding bot name config for each bots
adding custom.js
```

## BOX APPROVAL

``box approval`` is set as default, you can disable it on ``ryuko.json`` by setting the ``approval`` value into ``false``</br>

you can approve box by using ``approve`` command without using prefix, how to use? just type ``approve (box/remove) (uid/tid)``</br>

EXAMPLES : </br>

view approved list 
```txt 
approve list
```
add box from approved list 
```txt
approve box 4834812366643016
```
remove box from approved list 
```txt
approve remove 4834812366643016
```

## HOW TO ADD COMMANDS?
```js
module.exports.config = {
  name: "example", // command name.
  version: "1.0.0", // command version.
  permission: 0, // set to 1 if you want to set the permission into a group admins, set to 2 if you want to set the permission into a bot admins, set to 3 if you want to set the permission into a bot operators.
  credits: "", // who created the code
  description: "example", // command description.
  prefix: false, // set to true if you want to use the command with prefix, set to false if you want to use the commands without prefix.
  category: "example", // command category.
  usages: "example", // command ussage.
  cooldowns: 5, // 5 seconds command cooldown.
  dependencies: {
		"name": "version" // not required but if the command have a npm packages, you can type the package name and version to automatically install the package.
	}
};

module.exports.run = async ({api, event, args}) => {
  // start coding
}
```
