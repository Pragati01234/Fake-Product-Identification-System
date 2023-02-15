# Fake-Product-Identification-System
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
@import url('https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/css/bootstrap.min.css');
@import url('https://fonts.googleapis.com/css?family=Open+Sans:300,400,800');

@media (min-width: 500px) {
  .col-sm-6 {
    width: 50%;
  }
}
html, body {
  height: 100%;
  min-height: 18em;
}

.frontend-side {
  background-image: url("https://s3-us-west-2.amazonaws.com/s.cdpn.io/74452/website-code.png");
}

.uiux-side {
  background-image: url("https://s3-us-west-2.amazonaws.com/s.cdpn.io/74452/website-post-its.png");
}

.split-pane {
  padding-top: 1em;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
  height: 50%;
  min-height: 9em;
  font-size: 2em;
  color: white;
  font-family: 'Open Sans', sans-serif;
	font-weight:300;
;
}
@media(min-width: 500px) {
  .split-pane {
    padding-top: 2em;
    height: 100%;
  }
}
.split-pane > div {
  position: relative;
  top: 50%;
  -webkit-transform: translateY(-50%);
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
  text-align: center;
}
.split-pane > div .text-content {
  line-height: 1.6em;
  margin-bottom: 1em;
}
.split-pane > div .text-content .big {
  font-size: 2em;
}
.split-pane > div img {
  height: 1.3em;
}
@media (max-width: 500px) {
  .split-pane > div img {
    display:none;
  }
}
.split-pane button, .split-pane a.button {
  font-family: 'Open Sans', sans-serif;
	font-weight:800;
  background: none;
  border: 1px solid white;
  -moz-border-radius: 5px;
  -webkit-border-radius: 5px;
  border-radius: 5px;
  width: 15em;
  padding: 0.7em;
  font-size: 0.5em;
  -moz-transition: all 0.2s ease-out;
  -o-transition: all 0.2s ease-out;
  -webkit-transition: all 0.2s ease-out;
  transition: all 0.2s ease-out;
  text-decoration: none;
  color: white;
  display: inline-block;
	cursor: pointer;
}
.split-pane button:hover, .split-pane a.button:hover {
  text-decoration: none;
  background-color: white;
  border-color: white;
	cursor: pointer;
}
.uiux-side.split-pane button:hover, .split-pane a.button:hover {
  color: violet;
}
.frontend-side.split-pane button:hover, .split-pane a.button:hover {
  color: blue;
}

#split-pane-or {
  font-size: 2em;
  color: white;
  font-family: 'Open Sans', sans-serif;
  text-align: center;
  width: 100%;
  position: absolute;
  top: 50%;
  -webkit-transform: translateY(-50%);
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
}
@media (max-width: 925px) {
  #split-pane-or {
    top:15%;
  }
}
#split-pane-or > div img {
  height: 2.5em;
}
@media (max-width: 500px) {
  #split-pane-or {
    position: absolute;
    top: 50px;
  }
  #split-pane-or > div img {
    height:2em;
  }
}
@media(min-width: 500px) {
  #split-pane-or {
    font-size: 3em;
  }
}
.big {
  font-size: 2em;
}

#slogan {
  position: absolute;
  width: 100%;
  z-index: 100;
  text-align: center;
  vertical-align: baseline;
  top: 0.5em;
  color: white;
  font-family: 'Open Sans', sans-serif;
  font-size: 1.4em;
}
@media(min-width: 500px) {
  #slogan {
    top: 5%;
    font-size: 1.8em;
  }
}
#slogan img {
  height: 0.7em;
}
.bold {
	text-transform:uppercase;
}
.big {
	font-weight:800;
}

</style>
</head>
<body>

<div class='split-pane col-xs-12 col-sm-6 uiux-side'>
        <div>
          <img src='https://bit.ly/BCR-design'>
          <div class='text-content'>
            <div class="bold">Retailer</div>
            <div class='big'>Registration</div>
          </div>
          <a class='button' href="http://localhost:8080/createRetailer">
            REGISTER
          </a>
        </div>
      </div>

<div class='split-pane col-xs-12 col-sm-6 frontend-side'>
        <div>
          <img src='https://bit.ly/bcr-dev'>
          <div class='text-content'>
            <div class="bold">Generate</div>
            <div class='big'>QR Code</div>
          </div>
          <a class='button' href="http://localhost:8080/createCodes">
            GENERATE
          </a>
        </div>
      </div>

      <div id='split-pane-or'>
        <div>
          <img src='..\Pics\logo.png'>
        </div>
      </div>
<link href="//maxcdn.bootstrapcdn.com/bootstrap/4.1.1/css/bootstrap.min.css" rel="stylesheet" id="bootstrap-css">
<script src="//maxcdn.bootstrapcdn.com/bootstrap/4.1.1/js/bootstrap.min.js"></script>
<script src="//cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
<link href="C:\Users\Thomas AJ\Desktop\node_try\style1.css" rel="stylesheet" type="text/css">

<!doctype html>
<html lang="en">
<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Fonts -->
    <link rel="dns-prefetch" href="https://fonts.gstatic.com">
    <link href="https://fonts.googleapis.com/css?family=Raleway:300,400,600" rel="stylesheet" type="text/css">



    <link rel="icon" href="Favicon.png">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css">

    <title>AuthentiFi</title>
</head>
<body>
<nav class="navbar navbar-expand-lg navbar-light navbar-laravel">
    <div class="container">
    <a class="navbar-brand" href="http://localhost:8080/"  style="color:#1fa667">AuthentiFi</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav ml-auto">
            <li class="nav-item">
                <a class="nav-link" href="http://localhost:8080" style="color:#1fa667">Generate QR Code</a>
            </li>
        </ul>

    </div>
    </div>
</nav>

<main class="myform">
    <div  class="cotainer">
        <div class="row justify-content-center">
            <div class="col-md-8">
                    <div class="card">
                        <div style="background-color: #1fa667;color: #ffffff"  class="card-header">Retailer Registration</div>
                        <div class="card-body">
                            <form name="myform" onsubmit="return validform()" action="http://localhost:8080/retailerSignup" method="POST" >
                                <div class="form-group row">
                                    <label for="name" class="col-md-4 col-form-label text-md-right">Name</label>
                                    <div class="col-md-6">
                                        <input type="text" id="name" class="form-control" name="name">
                                    </div>
                                </div>

                                <div class="form-group row">
                                    <label for="email" class="col-md-4 col-form-label text-md-right">E-Mail Address</label>
                                    <div class="col-md-6">
                                        <input type="text" id="email" class="form-control" name="email">
                                    </div>
                                </div>

                                <div class="form-group row">
                                    <label for="location" class="col-md-4 col-form-label text-md-right">Location</label>
                                    <div class="col-md-6">
                                        <input type="text" id="location" class="form-control" name="location">
                                    </div>
                                </div>

                                <div class="form-group row">
                                    <label for="password" class="col-md-4 col-form-label text-md-right">Password</label>
                                    <div class="col-md-6">
                                        <input type="password" id="password" class="form-control" name="password">
                                    </div>
                                </div>

                                <div class="form-group row">
                                    <label for="pass" class="col-md-4 col-form-label text-md-right">Confirm Password</label>
                                    <div class="col-md-6">
                                        <input type="password" id="pass" class="form-control" name="pass">
                                    </div>
                                </div>

                                    <div class="col-md-6 offset-md-4">
                                        <button type="submit" class="btn btn-primary">
                                        Register
                                        </button>
                                    </div>
                                </div>
                            </form>
                        </div>
                    </div>
            </div>
        </div>
    </div>

</main>

<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"></script>
</body>
</html>
<link href="//maxcdn.bootstrapcdn.com/bootstrap/4.1.1/css/bootstrap.min.css" rel="stylesheet" id="bootstrap-css">
<script src="//maxcdn.bootstrapcdn.com/bootstrap/4.1.1/js/bootstrap.min.js"></script>
<script src="//cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
<link href="style1.css" rel="stylesheet" type="text/css">

<!doctype html>
<html lang="en">
<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Fonts -->
    <link rel="dns-prefetch" href="https://fonts.gstatic.com">
    <link href="https://fonts.googleapis.com/css?family=Raleway:300,400,600" rel="stylesheet" type="text/css">



    <link rel="icon" href="Favicon.png">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css">

    <title >AuthentiFi</title>
</head>
<body>
<nav class="navbar navbar-expand-lg navbar-light navbar-laravel">
    <div class="container">
    <a class="navbar-brand" href="http://localhost:8080/" style="color:#1fa667">AuthentiFi</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav ml-auto">
            <li class="nav-item">
                <a class="nav-link" href="http://localhost:8080/createRetailer" style="color:#1fa667">Retailer Registration</a>
            </li>
        </ul>

    </div>
    </div>
</nav>

<main class="myform">
    <div  class="cotainer">
        <div class="row justify-content-center">
            <div class="col-md-8">
                    <div class="card">
                        <div style="background-color: #1fa667;color: #ffffff"  class="card-header">Generate QR Codes</div>
                        <div class="card-body">
                            <form name="myform" onsubmit="return validform()" action="http://localhost:8080/QRCodeForManufacturer" method="POST" >

                                <div class="form-group row">
                                    <label for="brand" class="col-md-4 col-form-label text-md-right">Brand Name</label>
                                    <div class="col-md-6">
                                        <input type="text" id="brand" class="form-control" name="brand">
                                    </div>
                                </div>

                                <div class="form-group row">
                                    <label for="model" class="col-md-4 col-form-label text-md-right">Model</label>
                                    <div class="col-md-6">
                                        <input type="text" id="model" class="form-control" name="model">
                                    </div>
                                </div>

                                <div class="form-group row">
                                    <label for="description" class="col-md-4 col-form-label text-md-right">Description</label>
                                    <div class="col-md-6">
                                        <input type="text" id="description" class="form-control" name="description" style="height:100px">
                                    </div>
                                </div>

                                <div class="form-group row">
                                    <label for="manufacturerName" class="col-md-4 col-form-label text-md-right">Manufacturer Name</label>
                                    <div class="col-md-6">
                                        <input type="type" id="manufacturerName" class="form-control" name="manufacturerName">
                                    </div>
                                </div>

                                <div class="form-group row">
                                    <label for="manufacturerLocation" class="col-md-4 col-form-label text-md-right">Manufacturer Location</label>
                                    <div class="col-md-6">
                                        <input type="type" id="manufacturerLocation" class="form-control" name="manufacturerLocation">
                                    </div>
                                </div>

                                    <div class="col-md-6 offset-md-4">
                                        <button type="submit" class="btn btn-primary">
                                        Generate
                                        </button>
                                    </div>
                                </div>
                            </form>
                        </div>
                    </div>
            </div>
        </div>
    </div>

</main>

<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"></script>
</body>
</html>
<link href="//maxcdn.bootstrapcdn.com/bootstrap/4.1.1/css/bootstrap.min.css" rel="stylesheet" id="bootstrap-css">
<script src="//maxcdn.bootstrapcdn.com/bootstrap/4.1.1/js/bootstrap.min.js"></script>
<script src="//cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
<link href="C:\Users\Thomas AJ\Desktop\node_try\style1.css" rel="stylesheet" type="text/css">
<!------ Include the above in your HEAD tag ---------->

<!doctype html>
<html lang="en">
<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Fonts -->
    <link rel="dns-prefetch" href="https://fonts.gstatic.com">
    <link href="https://fonts.googleapis.com/css?family=Raleway:300,400,600" rel="stylesheet" type="text/css">



    <link rel="icon" href="Favicon.png">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css">

    <title>AuthentiFi</title>

    <script type="text/javascript" src="qrcode.js"></script>
    <style>
            h2 {
              text-align:center;
            }
            
            p {
              text-align:center;
            }
    </style>



</head>
<body> 
<nav class="navbar navbar-expand-lg navbar-light navbar-laravel">
    <div class="container">
    <a class="navbar-brand" href="file:///C:/Users/Thomas%20AJ/Desktop/node_try/main.html#">AuthentiFi</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
    </button>

    <!-- <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav ml-auto">
                <li class="nav-item">
                    <a class="nav-link" href="file:///C:/Users/Thomas%20AJ/Desktop/node_try/main.html#">Home</a>
                </li>
            </ul>
    </div> -->
    </div>
</nav>

    <div  class="cotainer">
        <div class="row justify-content-center">
            <div class="col-md-8">
                    <div class="card">
                        <div style="background-color: #1fa667;text-align:center;color: #ffffff"  class="card-header">Generated QR Code</div>
                        <div class="card-body">
                                <div class="container">
                                <div class="row">
                                    <div class="col-md-offset-2 col-md-8 col-lg-offset-3 col-lg-6">
                                        <div class="well details">  
                                            <div class="col-sm-12">
                                                <div class="col-xs-12 col-sm-8">
                                                    <h2 style="text-decoration:underline;"justify-content-center>Andrew Smith</h2>
                                                    <p justify-content-center><strong>Model: </strong>Senior Developer </p>
                                                    <p justify-content-center><strong>Description: </strong>Semantics </p>
                                                    <p><strong>Manufacturer Name: </strong>Data Visualization </p>
                                                    <p><strong>Manufacturer Location: </strong>Data Visualization </p>
                                                </div>
                                                <div class="col-xs-12 col-sm-4 col-lg-1 text-center">                        
                                                    <figure>
                                                            <div id="qrcode" style="width:500px; height:500px; margin-top:15px;"></div>

                                                            <script type="text/javascript">
                                                            function readTextFile(file)
                                                            {
                                                                var rawFile = new XMLHttpRequest();
                                                                rawFile.open("GET", file, false);
                                                                rawFile.onreadystatechange = function ()
                                                                {
                                                                    if(rawFile.readyState === 4)
                                                                    {
                                                                        if(rawFile.status === 200 || rawFile.status == 0)
                                                                        {
                                                                            var allText = rawFile.responseText;
                                                                            var qrcode = new QRCode(document.getElementById("qrcode"), {
                                                                                text:allText,
                                                                                width : 300,
                                                                                height : 300
                                                                            });
                                                                        }
                                                                    }
                                                                }
                                                                rawFile.send(null);
                                                            }
                                                            readTextFile("code.txt");
                                                            </script>      
                                                    </figure>
                                                </div>
                                            </div>                
                                        </div>
                                    </div>
                                </div>
                            </div>       
                        </div>    
                   </div>
                </div>
            </div>
        </div>
    </div>

</main>

<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"></script>
</body>
</html> 
* {
  box-sizing: border-box;
}

input[type=text], select, textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 4px;
  resize: vertical;
}

input[type=password], select, textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 4px;
  resize: vertical;
}


label {
  padding: 12px 12px 12px 0;
  display: inline-block;
}

input[type=submit] {
  background-color: #4CAF50;
  color: white;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  float: right;
}

input[type=submit]:hover {
  background-color: #45a049;
}

.container {
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 20px;
}

.col-25 {
  float: left;
  width: 25%;
  margin-top: 6px;
}

.col-75 {
  float: left;
  width: 75%;
  margin-top: 6px;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

/* Responsive layout - when the screen is less than 600px wide, make the two columns stack on top of each other instead of next to each other */
@media screen and (max-width: 600px) {
  .col-25, .col-75, input[type=submit] {
    width: 100%;
    margin-top: 0;
  }
}
