<!--//////// style///////////-->
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="http://www.w3schools.com/lib/w3.css">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Amatic+SC">
 
<style>
body, html {height: 100%}
body,h1,h2,h3,h4,h5,h6 {font-family: "Amatic SC", sans-serif}
.menu {display: none}
.bgimg {
    background-repeat: no-repeat;
    background-size: cover;
    background-image: url("http://www.mrwallpaper.com/wallpapers/forest-trees-waterfall.jpg");
    min-height: 90%;
}
</style>
<!--////////////// search///////////////-->
<?php
//Step1
  mysql_connect('localhost','gaby','gabyfg11')
 or die('Error connecting to MySQL server.');
  mysql_select_db("spring_database") or die(mysql_error());
?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
    <title>Search results</title>
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
    <link rel="stylesheet" type="text/css" href="style.css"/>
</head>
<body>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
    <title>Search results</title>
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
    <link rel="stylesheet" type="text/css" href="style.css"/>
</head>
<body>
<?php
if (isset($_GET['submit'])) {
if(isset($_GET['radio']))
{
echo "You have selected :".$_GET['radio'];  //  Displaying Selected Value
}}
    $option= $_GET['radio'];
    $query = $_GET['query']; 
    // gets value sent over search form
     
    $min_length = 3;
    // you can set minimum length of the query if you want
     
    if(strlen($query) >= $min_length){ // if query length is more or equal minimum length then
         
        $query = htmlspecialchars($query); 
        // changes characters used in html to their equivalents, for example: < to &gt;
         
        $query = mysql_real_escape_string($query);
        // makes sure nobody uses SQL injection
  //-------------Springs search------------------------//       
        if ($option=='Springs'){
        	$raw_results = mysql_query("SELECT * FROM Springs
            WHERE (`name` LIKE '%".$query."%') OR (`area` LIKE '%".$query."%')") or die(mysql_error());
             
        // * means that it selects all fields, you can also write: `id`, `title`, `text`
        // articles is the name of our table
         
        // '%$query%' is what we're looking for, % means anything, for example if $query is Hello
        // it will match "hello", "Hello man", "gogohello", if you want exact match use `title`='$query'
        // or if you want to match just full word so "gogohello" is out use '% $query %' ...OR ... '$query %' ... OR ... '% $query'
         
        	if(mysql_num_rows($raw_results) > 0){ // if one or more rows are returned do following
             
            	while($results = mysql_fetch_array($raw_results)){
            // $results = mysql_fetch_array($raw_results) puts data from database into array, while it's valid it does the loop
             
                	echo "<p><h3>".$results['name']."</h3>".$results['area']."</p>";
                // posts results gotten from database(title and text) you can also show id ($results['id'])
            	echo "<p><h3>".$results['latitude']."</h3>".$results['longitude']."</p>";
                $lat= $results['latitude'];
                $lon=$results['longitude'];
                }
             
        	}
        	else{ // if there is no matching rows do following
            	echo "No results";

        	}
         }
   //-------------------Park search--------//    
         if($option=='Park')
         {
         	$raw_results = mysql_query("SELECT * FROM Park
            WHERE (`name` LIKE '%".$query."%') OR (`area` LIKE '%".$query."%')") or die(mysql_error());
            if(mysql_num_rows($raw_results) > 0){
            	while($results = mysql_fetch_array($raw_results)){
            
             
                	echo "<p><h3>".$results['name']."</h3>".$results['area']."</p>";
               
            	}

            }
            else{ // if there is no matching rows do following
            	echo "No results";

        	}
             
         }
         if($option=='County')
         {
         	$raw_results = mysql_query("SELECT * FROM Region
            WHERE (`county` LIKE '%".$query."%') OR (`city` LIKE '%".$query."%')") or die(mysql_error());
            if(mysql_num_rows($raw_results) > 0){
            	while($results = mysql_fetch_array($raw_results)){
            
             
                	echo "<p><h3>".$results['county']."</h3>".$results['city']."</p>";
               
            	}

            }
            else{ // if there is no matching rows do following
            	echo "No results";

        	}
             
         }

    }
    else{ // if query length is less than minimum
        echo "Minimum length is ".$min_length;
    }
?>
<!--///////////////google map///////////////////--> 
<div id="googleMap" class="w3-grayscale-max" style="width:100%;height:400px;"></div>

<script src="https://maps.googleapis.com/maps/api/js"></script>
<script>
// Google Map Location from query 
var lat= <?php echo $lat?>;
var lon= <?php echo $lon?>;
var myCenter = new google.maps.LatLng(lat, lon);

function initialize() {
var mapProp = {
  center: myCenter,
  zoom: 12,
  scrollwheel: true,
  draggable: true,
  mapTypeId: google.maps.MapTypeId.ROADMAP
  };

var map = new google.maps.Map(document.getElementById("googleMap"),mapProp);

var marker = new google.maps.Marker({
  position: myCenter,
});

marker.setMap(map);
}

google.maps.event.addDomListener(window, 'load', initialize);

// Tabbed Menu
function openMenu(evt, menuName) {
  var i, x, tablinks;
  x = document.getElementsByClassName("menu");
  for (i = 0; i < x.length; i++) {
     x[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablink");
  for (i = 0; i < x.length; i++) {
     tablinks[i].className = tablinks[i].className.replace(" w3-red", "");
  }
  document.getElementById(menuName).style.display = "block";
  evt.currentTarget.firstElementChild.className += " w3-red";
}
document.getElementById("myLink").click();
</script>
</body>
</html>