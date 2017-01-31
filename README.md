<!DOCTYPE html>
<html>
<style>
body {font-family: "Lato", sans-serif;}

ul.tab {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
    border: 1px solid #ccc;
    background-color: #f1f1f1;
}

/* Float the list items side by side */
ul.tab li {float: left;}

/* Style the links inside the list items */
ul.tab li a {
    display: inline-block;
    color: black;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
    transition: 0.3s;
    font-size: 17px;
}

/* Change background color of links on hover */
ul.tab li a:hover {
    background-color: #ddd;
}

/* Create an active/current tablink class */
ul.tab li a:focus, .active {
    background-color: #ccc;
}

/* Style the tab content */
.tabcontent {
    display: none;
    padding: 6px 12px;
    border: 1px solid #ccc;
    border-top: none;
}
</style>
<body>

<p>Click on the links inside the tabbed menu:</p>

<ul class="tab">
  <li><a href="javascript:void(0)" class="tablinks" onclick="openCity(event, 'MathTeachers')">Math</a></li>
  <li><a href="javascript:void(0)" class="tablinks" onclick="openCity(event, 'Science')">Science</a></li>
  <li><a href="javascript:void(0)" class="tablinks" onclick="openCity(event, 'English')">English</a></li>
</ul>

<-------- first page---------->
<div data-role = “page” id = “MathTeachers”>
	<div data-role = “header”>
		<center><h1> Math Teachers Contact</h1></center>
</div>
<div data-role = “content”>
	<div id = “Riddle Contact”></div>
	<center>  
<h3>Riddle's Schedule</h3>
 		 <p>Email: john_riddle@ipsd.org</p> 
  		<p> open periods </p>
	<br> <br>
		<h3>Johnson's Schedule</h3>
  		<p>Email: natalie_johnson@ipsd.org</p> 
  		<p> open periods </p>

<br> <br>
		<h3>Trant's Schedule</h3>
 		 <p>Email: firstname_trant@ipsd.org</p> 
  		<p> open periods </p>

	<br> <br>
		 <h3>Whaley's Schedule</h3>
  		<p>Email: christopher_whaley@ipsd.org</p> 
 		 <p> open periods </p>


</center>
</div>
</div>

<script>
function openCity(evt, cityName) {
    var i, tabcontent, tablinks;
    tabcontent = document.getElementsByClassName("tabcontent");
    for (i = 0; i < tabcontent.length; i++) {
        tabcontent[i].style.display = "none";
    }
    tablinks = document.getElementsByClassName("tablinks");
    for (i = 0; i < tablinks.length; i++) {
        tablinks[i].className = tablinks[i].className.replace(" active", "");
    }
    document.getElementById(cityName).style.display = "block";
    evt.currentTarget.className += " active";
}
</script>
     
</body>
</html> 

