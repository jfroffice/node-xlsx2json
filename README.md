node-xlsx2json
=========

simple XLSX reader to JSON

Install
=======
```
npm install
```

Dependency
==========
[node-xlsx](https://github.com/mgcrea/node-xlsx)

Usage
=====
```
var rows = xlsx2json.load({
	filename: filename,
	sheetNumber: 0,
	minRow: 3,
	max: 250,  /* optional: limit max row */
	data: {
		lastname: 'H',
		firstname: 'G',
		email: 'P'
	}
});
```

Looping on each row
===================
```
for(var i=0; i<rows.length; i++) {
	var row = rows[i];
	var fullname = row.lastname + ' ' + row.firstname + ' ' + row.email;
	console.log(fullname);
}
```
