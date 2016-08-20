# exe-exiftool
A distribution of _exiftool.exe_. Current version is 10.25.

[![npm version](https://badge.fury.io/js/exiftool.exe.svg)](https://badge.fury.io/js/exiftool.exe)

## Usage
The module exports a path to the exiftool Windows executable.

```js
const exec = require('child_process').execFile;
const exiftool = require('exiftool.exe');

execFile(exiftool, ['-j', 'image.jpg'], (error, stdout, stderr) => {
	if (error) {
		console.error(`exec error: ${error}`);
		return;
	}
	console.log(`stdout: ${stdout}`);
	console.log(`stderr: ${stderr}`);
});
```

## Links
[exiftool](http://www.sno.phy.queensu.ca/~phil/exiftool/)

[sourceforge](https://sourceforge.net/projects/exiftool/)

[cpan](http://search.cpan.org/~exiftool/)

## License
Artistic License 2.0
