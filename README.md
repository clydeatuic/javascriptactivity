# Javascript Activity
* Javascript Overview
 * Javascript Basics
  * External JS
  * Internal JS
  * Variables
  * Document Object Models
  * Loops and Others
   * Activity
   '''
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
   '''
  <hr/>
  '''
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
  '''
* JSON [JSON link here](http://www.tutorialspoint.com/json/json_tutorial.pdf)
 * 
