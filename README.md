# Javascript Activity
* Javascript Overview
 * Javascript Basics
  * External JS
  * Internal JS
  * Variables
  * Document Object Models
  * Loops and Others
   * Activity
   ``` html
    <!-- index.html -->
    <!DOCTYPE html>
    <html>
    	<head>
    		<title>Javascript Activity</title>
    		<style>
    			#myTable {
    				background-color:yellow;
    			}
    		</style>
    	</head>
    	<body>
    		<h1 id='myTitle'>Title Heading</h1>
    		<div id='mySubTitle'>Subtitle</div>
    		<table border=1 id='myTable'></table>
    	</body>
    	<script type='text/javascript' src='js/script.js'></script>
    </html>
   ```
  <hr/>
  ``` js
  var _title = document.getElementById('myTitle');
  _title.innerHTML = "My New Title";
  
  var _subtitle = document.getElementById('mySubTitle');
  _subtitle.innerHTML = "My New SubTitle";
  
  var _table = document.getElementById('myTable');
  var row = 3;
  var col = 2;
  var arrNames = ['Reymar', 'Cindy', 'Kevin'];
  var arrGender = ['Male', 'Female', 'Male'];
  var index = 0;
  var html = "<thead><tr><th>Name</th><th>Gender</th></tr></thead>";
  html += "<tbody>";
  for(x=0;x<row;x++){
    html+="<tr>";
    for(y=0;y<col;y++){
  	html+="<td>"+arrNames[index]+"</td>";
  	html+="<td>"+arrGender[index]+"</td>";
    }
    html+="</tr>";
    index++;
  }
  html += "</tbody>";
  _table.innerHTML = html;
  ```
* JSON [JSON link here](http://www.tutorialspoint.com/json/json_tutorial.pdf)
 * Modify your previous javascript activity. Add the following html tags inside you 'index.html'
 ```html
 <!DOCTYPE html>
 <html>
 	<head>
 		<!-- title and styles here.. -->
 	</head>
 	<body>
 		<!-- same as previous index.html content -->
 		<hr/>
 		<table border=1 id='myTable2'></table>
 	</body>
 	<script type='text/javascript' src='js/script.js'></script>
 	<!-- include data.js external link script here.. -->
 </html>
 ```
 * Create a 'data.js' file
 ```js
 var students = { "MIT" : [
 { "name" : "Reymar", "gender" : "Male" },
 { "name" : "Cindy", "gender" : "Female" },
 { "name" : "Kevin", "gender" : "Male" }
 ]
} 

var htmlStudents = "<tr>";
for(i=0;i<students.MIT.length;i++)
{
 htmlStudents+="<td>";
 htmlStudents+="<table border='1' width=100 >";
 htmlStudents+="<tr><td><b>Name</b></td><td width=50>"+ students.MIT[i].name+"</td></tr>";
 htmlStudents+="<tr><td><b>Price</b></td><td width=50>"+ students.MIT[i].gender +"</td></tr>";
 htmlStudents+="</table>";
 htmlStudents+="</td>";
}
htmlStudents += "<tr>";

var _table2 = document.getElementById('myTable2');
_table2.innerHTML = htmlStudents;
 ```
* Update your previous activity and use bootstrap framework to make it more visually appealing.
``` html
    <!-- index.html -->
    <!DOCTYPE html>
    <html>
    	<head>
    		<title>Javascript Activity</title>
    		<link rel='stylesheet' href='bootstrap/dist/css/bootstrap.min.css'>
		    <script type='text/javascript' src='bootstrap/dist/js/bootstrap.min.js'></script>
		    
		    <!-- modify your tags to fit in bootstrap requirements -->
```    		
* Complete the table values
Name | Gender
------------ | -------------
Reymar | Male
Cindy | Female 
Kevin | Male
Dan | Male
Ed | Male
Glester | Male
Jeffrey | Male
