xlsx2json
=========

simple XLSX reader to JSON

Install
=======
```
npm install
```

Usage
=====
```
var data = xlsx2json.load({
	filename: filename,
	sheetNumber: 0,
	minRow: 3,
	max: 250,  /* limit max member */
	data: {
		lastname: 'H',
		firstname: 'G',
		email: 'P'
	}
});
```