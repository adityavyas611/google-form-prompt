# Get Google Forms as a prompt in terminal

This is a CLI based Google form, for scraping the questions in Command Line.

## Installation

Use the package manager [yarn](https://yarnpkg.com/lang/en/docs/install/#debian-stable) to install packages to run Google Forms.

```bash
yarn install
```

## Usage

```js
node index.js <google-form-id>
```

## Example

```js
const GoogleFormPrompt = require('./index.js');

const prompt = new GoogleFormPrompt({
    name: "Google Form",
    message: "Please provide the information:",
    form_id: process.argv[2],
});

prompt.run()
.then(res => console.log(res))
.catch(err => console.log(err));

```

More Examples can be found at [Link](https://github.com/adityavyas611/google-form-prompt)

This will fetch all the questions from the google form and will display as prompt.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.


## License
[MIT](https://choosealicense.com/licenses/mit/)