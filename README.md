# CSV-Generator-in-JavaScript

How to use:

Jsfiddle: https://jsfiddle.net/e0yjr4ns/2/

```
  function getsampleDataForCSV() {
   	var rows = [];
   	for (var i = 0; i < 100; i++) {
   		var thisData = {
   			Name: "name" + i,
   			School: "School" + i,
   			Address: "Address" + i
   		}
   		rows.push(thisData);
   	}
   	return rows;
   }
   var sampleData = getsampleDataForCSV();
   csvGenerator.exportCSV("test", sampleData, ["Name", "School", "Address"]);
   ```
