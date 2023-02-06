<!DOCTYPE html>
<html>
<head>	
	<title>Home</title>
	<meta name="robots" content="noindex,nofollow">
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	
<style>
header, footer{
	color:lightslategray;
	margin: 15px;
}
footer p{
	text-align: center;
	position: static;

}
nav { 
	background-color:lightslategray;
	height:30px;
	border-radius: 10px;
}	
li a{
	text-decoration: none;
}		
li a:visited{
	color: white;
	text-decoration: none;
}
li a:hover{
	color:white;
	font-weight: bold;
}
body {
    padding: 1rem;
	text-decoration: none;
	font-family: "Lucida Grande", "Lucida Sans Unicode", "Lucida Sans", "DejaVu Sans",   Verdana, "sans-serif";
}
h2 {
	text-align: left;
	color: lightblue;
}
article img {
	width: 99%;
	height: fit-content;
	border-radius: 30px;
}
fieldset{
	border-radius:7px;
	width: 300px;
	margin-bottom: 20px;
}
label{
    display: inline-block;
    width: 250px;
}
input{
	margin:10px;
}
ul{
	list-style-image: url('images/small-sun.jpg');
}
article li{
	margin:30px;
  }
.disclaimer{
	font-style: italic;
}
.grid-container article {
	margin: auto;
	border-radius: 45px;
	padding-top:10px;
	padding-left:20px;
	padding-right:20px;
	height:98%;
	border: thin solid lightblue;
	box-shadow: 4px 7px lightblue;
}	
.grid-container {
	display: grid;
	grid-template-columns: repeat(4, 2fr);
	flex-direction: column;
}	
.blank{
	width: 325px;
	height: 125px;
}
.blankprofile {
	width: 120px;
	height: 120px;
	border-radius: 10px;
	margin: 20px;
}
.navlist {
	display: inline-block;
	width: 150px;
	text-align: center;
	text-decoration: none;
	margin: 1px;
}
.buttons{							
	padding-left:100px;;
}
.modal {
	display: none;
	position: fixed;
	z-index: 1;
	padding-top: 100px;
	left: 0;
	top: 0;
	width: 100%;
	height: 100%;
	overflow: auto;
	background-color: rgba(0, 0, 0, 0.4);
}
.modal-content {
	position: relative;
	background-color: lightgrey;
	padding: 20px;
	margin: auto;
	width: 75%;
	-webkit-animation-name: animatetop;
	-webkit-animation-duration: 0.4s;
	animation-name: animatetop;
	animation-duration: 0.4s;
	border-radius:9px;
}
@-webkit-keyframes animatetop {
	from {
	  top: -300px;
	  opacity: 0;
	}
	to {
	  top: 0;
	  opacity: 1;
	}
}

.modal-content a:hover {
	color: lightblue;
	text-decoration: bold;
  }	

.modal-content a {
	color: white;
  }	

/* close modal button*/
.close {
	color: black;
	float: right;
	cursor: pointer;
	}

/*links on FAQ page*/
.myBtn_multi:hover {
	color:lightblue;
	cursor: pointer;
}
	
	

	@media screen and (min-width: 280px) {
		.grid-container {
		  grid-auto-rows: minmax(300px, auto);
		  grid-template-columns: repeat(1, 3fr);
		  flex-direction: column;
		  grid-gap:30px;
		}
		#toggle {
		  display: block;
		  position: absolute;
		  top: 165px;
		  left: 50px;
		  z-index: 1;
		  -webkit-user-select: none;
		  user-select: none;
		}
	  
		#toggle a {
		  text-decoration: none;
		  color: black;
		  transition: color 0.2s ease;
		}
	  
		#toggle a:hover {
		  color: whitesmoke;
		}
	  
		#toggle input {
		  display: block;
		  width: 30px;
		  height: 30px;
		  position: absolute;
		  left: -5px;
		  cursor: pointer;
		  opacity: 0;
		  z-index: 2;
		  -webkit-touch-callout: none;
		}
	  
		#toggle span {
		  display: block;
		  width: 30px;
		  height: 3px;
		  margin-bottom: 6px;
		  position: relative;
		  background: lightgrey;
		  border-radius: 7px;
		  z-index: 1;
		  transform-origin: 0px 0px;
		  transition: transform 0.5s cubic-bezier(1.0, 0.125, 0.05, 10.0),
					  background 0.5s cubic-bezier(1.0, 0.125, 0.05, 10.0),
					  opacity 0.55s ease;
		}
	  
		#toggle span:first-child {
		  transform-origin: 0% 0%;
		}
	  
		#toggle span:nth-last-child(2) {
		  transform-origin: 0% 100%;
		}
	  
		#toggle input:checked ~ span {
		  opacity: 1;
		  transform: rotate(45deg) translate(-2px, -1px);
		  background: black;
		}
	  
		#toggle input:checked ~ span:nth-last-child(3) {
		  opacity: 0;
		  transform: rotate(0deg) scale(0.2, 0.2);
		}
	  
		#toggle input:checked ~ span:nth-last-child(2) {
		  transform: rotate(-45deg) translate(0, -1px);
		}
	  
		#menu {
		  position: absolute;
		  width: 110px;
		  margin: -50px 0 0 -50px;
		  padding: 50px;
		  padding-top: 80px;
		  border-radius: 9px;
		  background: lightgrey;
		  list-style-type: none;
		  -webkit-font-smoothing: antialiased;
		  transform-origin: 0% 0%;
		  transform: translate(-100%, 0);
		  transition: transform 0.5s cubic-bezier(1.0, 0.2, 0.05, 1.0);
		}
	
		#menu li {
		  padding: 10px 0;
		  font-size: 20px;
	    }
	  
	  	#toggle input:checked ~ ul {
		  transform: none;
	    }

	}	  

	@media screen and (min-width: 650px) {
		.grid-container {
			grid-auto-rows: minmax(300px, auto);
			grid-template-columns: repeat(2, 3fr);
			flex-direction: column;
		}
	}
	  
	@media screen and (min-width: 960px) {
		.grid-container {
 			grid-auto-rows: minmax(300px, auto);
  			grid-template-columns: repeat(3, 3fr);
  			flex-direction: column;
		}

	} 
</style>
</head>

<body>

<header>
<div class="logo">
	<a href="index.html"><img src="images/shine-logo.jpg" alt="SHINE Logo" width="100" height="100"></a>
</div>
</header>
			
<nav role="navigation">
	<div id="toggle">
	  
	  <input type="checkbox" />
	  <span></span>
	  <span></span>
	  <span></span>
	  
	  <ul id="menu">
		<li class="navlist"><a href="index.html">Home</a></li>
		<li class="navlist"><a href="pages/AboutUs.html">About Us</a></li>
	    <li class="navlist"><a href="pages/Volunteer.html">Volunteer</a></li>
		<li class="navlist"><a href="pages/FAQ.html">FAQ</a></li>
		<li class="navlist"><a href="pages/Contact.html">Contact</a></li>
	  </ul>
	</div>
</nav>


<article><p class="disclaimer">This site was built for a class project and is not associated with any actual organization.</p></article>


 <main class="grid-container">

	<article> 
	  <h2>How private citizens are taking Rhode Island’s housing crisis into their own hands</h2>
	  <p>Residents who never envisioned their lives on the streets are being pushed out of homes and others are becoming chronically unhoused. David Gerard O’Connor is trying to help with Operation Hunker Down, a makeshift shelter he opened on his own.</p>
	  <a href="https://www.bostonglobe.com/2022/02/15/metro/ris-housing-crisis-becomes-critical-private-citizens-are-addressing-it-their-own/"><img src="https://bostonglobe-prod.cdn.arcpublishing.com/resizer/4NpUScppm_D_MdhrvhJ6os9vtng=/600x0/cloudfront-us-east-1.images.arcpublishing.com/bostonglobe/2WEQ3RCSBIJC37R2C6IJRGIFLI.jpg" alt="SHINE Logo" width="100" height="200"></a>
	  <p><i>Source: </i>Boston Globe</p>	
	</article>
	
	<article>
	  <h2>Testimonials</h2>
	  <p>“They need a lot. But they are doing the work. They are sheltering people. They’re the ones getting it done right now.”</p> 
	  <p><i>-Ehren Hunt, Housing Specialist at Tri-County Community Action Agency</i></p>
	</article>
	
	<article>
      <h2>Services</h2>
	
	  <p><span>Here are some resources we offer:</span></p>
	
	  <ul>
	   <li>Connecting homeowners with skilled workers adding value to their homes</li>
	   <li>Providing affordable housing for boarders</li>	
	   <li>WrapAround Services</li>
	   <li>Recovery Services</li>
	   <li>Safety, Shelter & Community</li>
	  </ul>
	</article>
	
 </main>

   <footer>
	<p>
		&copy 2022 This site is under construction. 
	</p>		
   </footer>
		
  </body>
		
</html>
