# Entropy Calculator

Entropy Calculator for the language-dependent strings with support for 10+ languages.
* The tool is language-space sensitive. Use with proper language option.

## Installation

Use the package manager [npm](https://www.npmjs.com/package/entropy_calculator) to install

```bash
npm i entropy_calculator
```

## Feautures
Supports 10+ languages in the current version. All the supported languages are as follows:
* Chinese(中国人)
* Devnagari(देवनागरी)
* English
* French(Français)
* German(Deutsch)
* Greek(ελληνικά)
* Hebrew(עִברִית)
* Hinglish(HIndi+English)
* Modern Latin
* Russian(Русский)
* Spanish(Español)

## Usage

```javascript
const test  = require("entropy_calculator");

//Allowed language options ["chinese", "devanagari", "english", "french", "german", "greek","hebrew","hinglish","latin", "russian", "spanish"]
//const result = test("<PASSWORD_STRING>", "<LANGUAGE>");

const result = test("martes h71 panda sigla cereo", "spanish"); 
console.log(result); // returns 174

result = test("neon 95th prissy ib read tern", "english");
console.log(result); // returns 247

result = test("тайна скарб литьЄ завет боком форма фильм", "russian");
console.log(result); // returns 177

```
#
## Note
Selection of the correct language, while invoking the function, is necessary for the proper calculation of the entropy.
For e.g. with string _archer carol cody blimp skit_ the correct language option is _english_. Any other language option would result in incorrect entropy.

## Constraints
* Supports online single language strings.
* Mixing of the language is not supported in the current version.
* Arabic numbers [0-9] is allowed with all the input string.
