# CSV-Generator-in-JavaScript

This utility convers an object array to a CSV file. Each object represents a row in the CSV file. 

Jsfiddle: https://jsfiddle.net/e0yjr4ns/2/

How to use:

To generate a csv file, The first step is to include the csv-generator.js in your project and then calling exportCSV method with three parameters: CSV file name, object array and column array.  

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
