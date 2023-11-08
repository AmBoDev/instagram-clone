<!DOCTYPE html> 
<html lang="en"> 
<head> 
	<style>
    * { 
margin: 0; 
padding: 0; 
box-sizing: border-box; 
} 

body { 
  background: rgb(var(--ig-primary-background));
    color: rgb(var(--ig-primary-text));
    font-family: var(--font-family-system);
    font-size: var(--system-14-font-size);
    line-height: var(--system-14-line-height);
    margin: 0;
    overflow-y: visible
}


.navbar { 
position: sticky; 
z-index: 100000; 
display: flex; 
align-items: center; 
justify-content: center; 
background: rgb(var(--ig-primary-background)); 
width: 100%; 
border: 1px solid rgb(218, 217, 217); 
} 

.navbar .container { 
/* background-color: #555; */
padding: 15px 0; 
width: 75%; 
display: flex; 
align-items: center; 
justify-content: space-between; 
/* margin: 0 auto; */
} 

.container .logo { 
display: inline-block; 
cursor: pointer; 

} 

.searchbar { 
width: -10%; 
text-align: end; 
} 

.searchbar input { 
background-color: #fafafa; 
padding: 5px; 
text-indent: 21px; 
outline: none; 
border: 1px solid rgb(218, 217, 217); 
border-radius: 2px; 
color: rgb(77, 77, 77); 
} 

.searchbar img { 
position: absolute; 
margin-left: -10.5rem; 
margin-top: 0.25rem; 
} 

.searchbar input::placeholder { 
font-weight: lighter; 
color: rgb(172, 172, 172); 
} 

.nav-links { 
font-weight: lighter; 
color: rgb(172, 172, 172); 
/* background: #333 ; */
} 

.nav-group .nav-item { 
list-style-type: none; 
margin: 0 8px; 
} 
.bottom-right {
  position: absolute;
  top: 18px;
  left: 16px;
}
.bottom-left
{
	position: absolute;
  bottom: 18px;
  right:16px;
}
.nav-group .nav-item a { 
font-size: 22px; 
display: block; 
color: black; 
} 

.nav-group { 
display: flex; 
align-items: center; 
justify-content: center; 
} 

.action .profile { 
position: relative; 
width: 25px; 
height: 25px; 
border-radius: 50%; 
overflow: hidden; 
cursor: pointer; 
display: flex; 
align-items: center; 
justify-content: center; 
} 

.action .profile img { 
width: 100%; 
height: 100%; 
object-fit: cover; 
} 

main { 
width: 100%; 
display: flex; 
align-items: center; 
justify-content: center; 
} 

main .container { 
position: relative; 
margin-top: 60px; 
width: 75%; 
display: flex; 
align-items: flex-start; 
justify-content: space-between; 
/* background: #ddd; */
} 

.col-9 { 
width: 65%; 
margin-top: 30px; 
} 

.statuses { 
margin-bottom: 30px; 
width: 100%; 
background-color: #fff; 
display: flex; 
align-items: center; 
justify-content: start; 
padding: 20px 0; 
border-radius: 2px; 
border: 1px solid rgb(218, 217, 217); 
overflow: auto; 
} 

.statuses .status { 
display: inline-block; 
border-radius: 50%; 
overflow: auto; 
width: 70px; 
height: 70px; 
min-width: 70px; 
min-height: 70px; 
background: linear-gradient(to right, red, orange); 
padding: 2px; 
margin-left: 15px; 
cursor: pointer; 
} 

.statuses .status .image { 
position: relative; 
width: 100%; 
height: 100%; 
border-radius: 50%; 
overflow: hidden; 
cursor: pointer; 
display: flex; 
align-items: center; 
justify-content: center; 
border: 2px solid white; 
} 

.statuses .status img { 
width: 100%; 
height: 100%; 
object-fit: cover; 
} 

.col-3 { 
width: 33%; 
position: -webkit-sticky; 
position: sticky; 
top: 90px; 
} 

.col-3 h4 { 
color: rgb(100, 100, 100); 
} 

.col-3 .card { 
margin-bottom: 20px; 
position: relative; 
width: 100%; 
/* min-height: 400px; */
display: inline-block; 
} 

.col-3 .card .top { 
padding: 10px 0px; 
display: flex; 
justify-content: space-between; 
align-items: center; 
} 

.col-3 .card .top a { 
color: #1d92ff; 
} 

.col-3 .card .bottom { 
padding: 10px 20px; 
} 

.col-3 .card .top .userDetails { 
width: 100%; 
display: flex; 
align-items: center; 
} 

.col-3 .card .top .userDetails h3 { 
font-size: 16px; 
color: #4d4d4f; 
font-weight: 500; 
line-height: 1em; 
} 

.col-3 .card .top .userDetails h3 span { 
font-size: 0.75em; 
} 

.col-3 .card .top .userDetails h3 span { 
font-size: 0.75em; 
} 

.col-9 .card { 
margin-bottom: 20px; 
position: relative; 
width: 100%; 
/* min-height: 400px; */
display: inline-block; 
border: 1px solid rgba(7, 7, 7, 0.24); 
} 

.col-9 .card .top { 
padding: 10px 20px; 
display: flex; 
justify-content: space-between; 
align-items: center; 
} 

.col-9 .card .bottom { 
padding: 10px 20px; 
} 

.col-9 .card .top .userDetails { 
width: 100%; 
display: flex; 
align-items: center; 
} 

.profilepic { 
display: inline-block; 
cursor: pointer; 
} 

.profilepic .profile_img { 
display: flex; 
align-items: center; 
justify-content: center; 
border-radius: 50%; 
overflow: hidden; 
width: 30px; 
height: 30px; 
background: linear-gradient(to right, red, orange); 
padding: 2px; 
margin-right: 8px; 
cursor: pointer; 
} 

.profilepic .profile_img .image { 
position: relative; 
width: 100%; 
height: 100%; 
border-radius: 50%; 
overflow: hidden; 
cursor: pointer; 
display: flex; 
align-items: center; 
justify-content: center; 
border: 2px solid white; 
} 

.profilepic .profile_img img { 
width: 100%; 
height: 100%; 
object-fit: cover; 
} 

.cover { 
position: absolute; 
top: 0; 
left: 0; 
width: 100%; 
height: 100%; 
object-fit: cover; 
} 

.col-9 .card .top .userDetails h3 { 
/* width: 100%; */
font-size: 16px; 
color: #4d4d4f; 
font-weight: 500; 
line-height: 1em; 
} 

.col-9 .card .top .userDetails h3 span { 
font-size: 0.75em; 
} 

.col-9 .card .top .userDetails h3 span { 
font-size: 0.75em; 
} 

.dot { 
transform: scale(0.6); 
cursor: pointer; 
} 

.imgBx { 
position: relative; 
width: 100%; 
min-height: 600px; 
margin: 10px 0 15px; 
} 

.actionBtns { 
display: flex; 
justify-content: space-between; 
align-items: center; 
} 

.actionBtns svg { 
cursor: pointer; 
} 

.actionBtns .left svg { 
margin-right: 8px; 
} 

.likes { 
font-weight: 500; 
margin-top: 5px; 
font-size: 14px; 
color: #4d4d4f; 
} 

.message { 
font-weight: 400; 
margin-top: 5px; 
font-size: 14px; 
color: #777; 
line-height: 1.5em; 
} 

.message b { 
color: #262626; 
} 

.message span { 
cursor: pointer; 
color: #1d92ff; 
} 

.comments { 
margin-top: 10px; 
font-weight: 400; 
color: #999; 
} 

.addComments { 
display: flex; 
align-items: center; 
margin-top: 20px; 
border-top: 1px solid #ddd; 
padding: 10px 0; 
} 

.addComments a { 
color: #1d92ffcb; 
font-weight: 500; 
} 

.addComments .reaction { 
position: relative; 
font-size: 1.3rem; 
margin-right: 10px; 
color: rgb(88, 88, 88); 
} 

input.text { 
width: 100%; 
border: none; 
outline: none; 
font-weight: 400; 
font-size: 14px; 
color: #262626; 
background: none; 
} 

input.text::placeholder { 
color: #777; 
} 

.postTime { 
margin-top: 8px; 
font-weight: lighter; 
color: rgb(163, 163, 163); 
font-size: 12px; 
text-transform: uppercase; 
} 

a { 
text-decoration: none; 
} 

.hidden { 
display: none; 
} 

@media screen and (max-width: 1000px) { 
.col-9 { 
	width: 100%; 
	background: #fafafa; 
} 

.col-3 { 
	display: none; 
} 
} 

@media screen and (max-width: 600px) { 
.container { 
	width: 100% !important; 
} 

.navbar .container { 
	padding: 15px 10px !important; 
} 

.col-9 { 
	margin-top: 4px; 
	min-width: 100%; 
} 

.statuses { 
	margin-bottom: 0px; 
} 

.col-9 .card { 
	margin-bottom: 0px; 
	width: 100%; 
	border: none; 
} 

.imgBx { 
	position: relative; 
	width: 100%; 
	min-height: 400px; 
	margin: 10px 0 15px; 
} 

.searchbar { 
	display: none; 
} 
} 

.footer .footer-section { 
margin-left: 0.5rem; 
color: #999999; 
font-size: 14px; 
font-family: sans-serif; 
} 

.footer a:hover { 
color: #ff0000; 
}
</style>
	<title>Instagram Clone</title> 
</head> 
<body> 

<!--  Header section Starts from here -->
	<header> 
		<nav class="navbar"> 
			<div class="container"> 
				<div class="logo"> 
					<a href="#"> 
					<img src= 
"OIP.jpg"
						alt="img1"> 
					</a> 
				</div> 
        <div class="bottom-right">
          <h2>
          <i>
            Instagram
</i>
</h2>
</div>
				<div class="searchbar"> 
					<input type="text"
						placeholder="Search"> 
					<img src= 
"https://media.geeksforgeeks.org/wp-content/uploads/20220609093658/search-200x200.png"
						height="18"
						alt="img2"> 
				</div> 
				<div class="nav-links"> 
					<ul class="nav-group"> 
						<li class="nav-item"> 
							<a href="#"> 
								<i class="fas fa-home"></i> 
							</a> 
						</li> 
						<li class="nav-item"> 
							<a href=""> 
								<i class="fab fa-facebook-messenger"></i> 
							</a> 
						</li> 
						<li class="nav-item"> 
							<a href=""> 
								<i class="far fa-compass"></i> 
							</a> 
						</li> 
						<li class="nav-item"> 
							<a href=""> 
								<i class="far fa-heart"></i> 
							</a> 
						</li> 
						<li class="nav-item"> 
							<div class="action"> 
								<div class="profile"
									onclick="menuToggle()"> 
									<img src= 
"1.jpg"
										alt="user Avatar"> 
								</div> 
							</div> 
						</li> 
					</ul> 
				</div> 
			</div> 
		</nav> 
	</header> 
	
	<!-- Code for Showing the Status -->
	<main> 
		<div class="container"> 
			<div class="col-9"> 
				<div class="statuses"> 
					<div class="status"> 
						<div class="image">
								
							<img src= 
"1.jpg"
								alt="img3"> 
							
                
						</div>
						
					</div> 
         
					<div class="status"> 
						<div class="image"> 
							<img src= 
"2.jpg"
								alt="img4"> 
						</div> 
					</div> 
					<div class="status"> 
						<div class="image"> 
							<img src= 
"3.jpg"
								alt="img5"> 
						</div> 
					</div> 
					<div class="status"> 
						<div class="image"> 
							<img src= 
"4.jpg"
								alt="img6"> 
						</div> 
					</div> 
					<div class="status"> 
						<div class="image"> 
							<img src= 
"5.jpg"
								alt="img7"> 
						</div> 
					</div> 
					<div class="status"> 
						<div class="image"> 
							<img src= 
"6.jpg"
								alt="img8"> 
						</div> 
					</div> 
				</div> 
				
			<!-- Code for viewing the Post -->
				<div class="card"> 
					<div class="top"> 
						<div class="userDetails"> 
							<div class="profilepic"> 
								<div class="profile_img"> 
									<div class="image"> 
										<img src= 
"2.jpg"
											alt="img8"> 
									</div> 
								</div> 
							</div> 
							<h3>Amirnder singh 
								<br> 
								<span>prayagraj, India</span> 
						</h3> 
						</div> 
						<div> 
							<span class="dot"> 
								<i class="fas fa-ellipsis-h"></i> 
							</span> 
						</div> 
					</div> 
					<div class="imgBx"> 
						<video width="600" height="540" controls autoplay>
							<source src="8.mp4" type="video/mp4">
						</video>
					</div> 
					<div class="bottom"> 
						<div class="actionBtns"> 
							<div class="left"> 
								<span class="heart"
									onclick="addlike()"> 
									<span> 
										<svg aria-label="Like"
											color="#262626"
											fill="#262626"
											height="24"
											role="img"
											viewBox="0 0 48 48"
											width="24"> 
											<!-- Coordinate path -->

											<path
												d="M34.6 6.1c5.7 0 10.4 5.2 10.4 
												11.5 0 6.8-5.9 11-11.5 16S25 41.3 24 
												41.9c-1.1-.7-4.7-4-9.5-8.3-5.7-5-11.5-9.2-11.5-16C3 
												11.3 7.7 6.1 13.4 6.1c4.2 0 6.5 2 8.1 4.3 
												1.9 2.6 2.2 3.9 2.5 3.9.3 0 .6-1.3 2.5-3.9 
												1.6-2.3 3.9-4.3 8.1-4.3m0-3c-4.5 0-7.9 
												1.8-10.6 5.6-2.7-3.7-6.1-5.5-10.6-5.5C6 3.1 
												0 9.6 0 17.6c0 7.3 5.4 12 10.6 16.5.6.5 1.3 
												1.1 1.9 1.7l2.3 2c4.4 3.9 6.6 5.9 7.6 6.5.5.3 
												1.1.5 1.6.5.6 0 1.1-.2 1.6-.5 1-.6 2.8-2.2 
												7.8-6.8l2-1.8c.7-.6 1.3-1.2 2-1.7C42.7 29.6 
												48 25 48 17.6c0-8-6-14.5-13.4-14.5z"> 
											</path> 
										</svg> 
									</span> 
								</span> 
								<svg aria-label="Comment"
									class="_8-yf5 "
									color="#262626"
									fill="#262626"
									height="24"
									role="img"
									viewBox="0 0 48 48"
									width="24"> 
									
							<!-- Coordinate path -->
									<path clip-rule="evenodd"
										d="M47.5 46.1l-2.8-11c1.8-3.3 2.8-7.1 2.8-11.1C47.5 
										11 37 .5 24 .5S.5 11 .5 24 11 47.5 24 47.5c4 0 
										7.8-1 11.1-2.8l11 2.8c.8.2 1.6-.6 1.4-1.4zm-3-22.1c0 
										4-1 7-2.6 10-.2.4-.3.9-.2 1.4l2.1 
										8.4-8.3-2.1c-.5-.1-1-.1-1.4.2-1.8 1-5.2 2.6-10 
										2.6-11.4 0-20.6-9.2-20.6-20.5S12.7 3.5 24 3.5 
										44.5 12.7 44.5 24z" 
										fill-rule="evenodd"> 
								</path> 
								</svg> 
								<svg aria-label="Share Post"
									class="_8-yf5 "
									color="#262626"
									fill="#262626"
									height="24"
									role="img"
									viewBox="0 0 48 48"
									width="24"> 
									<path
										d="M47.8 3.8c-.3-.5-.8-.8-1.3-.8h-45C.9 3.1.3 
										3.5.1 4S0 5.2.4 5.7l15.9 15.6 5.5 22.6c.1.6.6 
										1 1.2 1.1h.2c.5 0 1-.3 
										1.3-.7l23.2-39c.4-.4.4-1 .1-1.5zM5.2 
										6.1h35.5L18 18.7 5.2 6.1zm18.7 
										33.6l-4.4-18.4L42.4 8.6 23.9 39.7z"> 
									</path> 
								</svg> 
							</div> 
							<div class="right"> 
								<svg aria-label="Save"
									class="_8-yf5 "
									color="#262626"
									fill="#262626"
									height="24"
									role="img"
									viewBox="0 0 48 48"
									width="24"> 
															
								<!-- Coordinate path -->
									<path
										d="M43.5 48c-.4 0-.8-.2-1.1-.4L24 29 5.6 
										47.6c-.4.4-1.1.6-1.6.3-.6-.2-1-.8-1-1.4v-45C3 .7 
										3.7 0 4.5 0h39c.8 0 1.5.7 1.5 1.5v45c0 .6-.4 
										1.2-.9 1.4-.2.1-.4.1-.6.1zM24 26c.8 
										0 1.6.3 2.2.9l15.8 16V3H6v39.9l15.8-16c.6-.6 
										1.4-.9 2.2-.9z"> 
									</path> 
								</svg> 
							</div> 
						</div> 
						<a href="#"> 
							<p class="likes">203 likes</p> 

						</a> 
						<a href="#"> 
							<p class="message"> 
							<b>narendra Modi</b> 
							</p> 

						</a> 
						<a href="#"> 
							<h4 class="comments">View all 32 comments</h4> 
						</a> 
						<a href="#"> 
							<h5 class="postTime">2 hours ago</h5> 
						</a> 
						<div class="addComments"> 
							<div class="reaction"> 
								<h3> 
								<i class="far fa-smile"></i> 
								</h3> 
							</div> 
							<input type="text"
								class="text"
								placeholder="Add a comment..."> 
							<a href="#">Post</a> 
						</div> 
					</div> 
				</div> 
				<div class="card"> 
					<div class="top"> 
						<div class="userDetails"> 
							<div class="profilepic"> 
								<div class="profile_img"> 
									<div class="image"> 
										<img src= 
"3.jpg"
											alt="img9"> 
									</div> 
								</div> 
							</div> 
							<h3>aviral singhal<br> 
							<span>Delhi, India</span> 
							</h3> 
						</div> 
						<div> 
							<span class="dot"> 
								<i class="fas fa-ellipsis-h"></i> 
							</span> 
						</div> 
					</div> 
					<div class="imgBx"> 
						<img src= 
"https://static.sportskeeda.com/wp-content/uploads/2016/03/virat-kohli-1458411816-800.jpg"
							alt="post-1" class="cover"> 
					</div> 
					<div class="bottom"> 
						<div class="actionBtns"> 
							<div class="left"> 
								<span class="heart"
									onclick="addlike()"> 
									<span> 
										<svg aria-label="Like"
											color="#262626"
											fill="#262626"
											height="24"
											role="img"
											viewBox="0 0 48 48"
											width="24"> 
								<!-- Coordinate path -->

											<path
												d="M34.6 6.1c5.7 0 10.4 5.2 10.4 11.5 
												0 6.8-5.9 11-11.5 16S25 41.3 24 
												41.9c-1.1-.7-4.7-4-9.5-8.3-5.7-5-11.5-9.2-11.5-16C3 
												11.3 7.7 6.1 13.4 6.1c4.2 0 6.5 2 8.1 
												4.3 1.9 2.6 2.2 3.9 2.5 3.9.3 0 .6-1.3 
												2.5-3.9 1.6-2.3 3.9-4.3 8.1-4.3m0-3c-4.5 
												0-7.9 1.8-10.6 5.6-2.7-3.7-6.1-5.5-10.6-5.5C6 
												3.1 0 9.6 0 17.6c0 7.3 5.4 12 10.6 
												16.5.6.5 1.3 1.1 1.9 1.7l2.3 2c4.4 3.9 
												6.6 5.9 7.6 6.5.5.3 1.1.5 1.6.5.6 0 
												1.1-.2 1.6-.5 1-.6 2.8-2.2 
												7.8-6.8l2-1.8c.7-.6 1.3-1.2 2-1.7C42.7 
												29.6 48 25 48 17.6c0-8-6-14.5-13.4-14.5z"> 
											</path> 
										</svg> 
									</span> 
								</span> 
								<svg aria-label="Comment"
									class="_8-yf5 "
									color="#262626"
									fill="#262626"
									height="24"
									role="img"
									viewBox="0 0 48 48"
									width="24"> 
									<path clip-rule="evenodd"
											
							<!-- Coordinate path -->
						
										d="M47.5 46.1l-2.8-11c1.8-3.3 2.8-7.1 
										2.8-11.1C47.5 11 37 .5 24 .5S.5 11 .5 24 11 
										47.5 24 47.5c4 0 7.8-1 11.1-2.8l11 2.8c.8.2 
										1.6-.6 1.4-1.4zm-3-22.1c0 4-1 7-2.6 10-.2.4-.3.9-.2 
										1.4l2.1 8.4-8.3-2.1c-.5-.1-1-.1-1.4.2-1.8 
										1-5.2 2.6-10 2.6-11.4 0-20.6-9.2-20.6-20.5S12.7 
										3.5 24 3.5 44.5 12.7 44.5 24z" 
										fill-rule="evenodd"></path> 
								</svg> 
								<svg aria-label="Share Post"
									class="_8-yf5 "
									color="#262626"
									fill="#262626"
									height="24"
									role="img"
									viewBox="0 0 48 48"
									width="24"> 
									<path
										d="M47.8 3.8c-.3-.5-.8-.8-1.3-.8h-45C.9 3.1.3 
										3.5.1 4S0 5.2.4 5.7l15.9 15.6 5.5 22.6c.1.6.6 
										1 1.2 1.1h.2c.5 0 1-.3 1.3-.7l23.2-39c.4-.4.4-1 .1-1.5zM5.2 
										6.1h35.5L18 18.7 5.2 6.1zm18.7 33.6l-4.4-18.4L42.4 
										8.6 23.9 39.7z"> 
									</path> 
								</svg> 
							</div> 
							<div class="right"> 
								<svg aria-label="Save"
									class="_8-yf5 "
									color="#262626"
									fill="#262626"
									height="24"
									role="img"
									viewBox="0 0 48 48"
									width="24"> 
							<!-- Coordinate path -->

									<path
										d="M43.5 48c-.4 0-.8-.2-1.1-.4L24 29 5.6 
										47.6c-.4.4-1.1.6-1.6.3-.6-.2-1-.8-1-1.4v-45C3 .7 
										3.7 0 4.5 0h39c.8 0 1.5.7 1.5 1.5v45c0 .6-.4 
										1.2-.9 1.4-.2.1-.4.1-.6.1zM24 26c.8 0 1.6.3 
										2.2.9l15.8 16V3H6v39.9l15.8-16c.6-.6 1.4-.9 2.2-.9z"> 
									</path> 
								</svg> 
							</div> 
						</div> 
					
					<!-- Adding number of like and name of people -->

						<a href="#"> 
							<p class="likes">119 likes</p> 

						</a> 
						<a href="#"> 
							<p class="message"> 
							<b>mukul Agarwal</b> 
							</p> 

						</a> 
						<a href="#"> 
							<h4 class="comments">View all 20 comments</h4> 
						</a> 
						<a href="#"> 
							<h5 class="postTime">4 hours ago</h5> 
						</a> 
						<div class="addComments"> 
							<div class="reaction"> 
								<h3><i class="far fa-smile"></i></h3> 
							</div> 
							<input type="text"
								class="text"
								placeholder="Add a comment..."> 
							<a href="#">Post</a> 
						</div> 
					</div> 
				</div> 
				<div class="card"> 
					<div class="top"> 
						<div class="userDetails"> 
							<div class="profilepic"> 
								<div class="profile_img"> 
									<div class="image"> 
										<img src="5.jpg"
											alt="img10"> 
									</div> 
								</div> 
							</div> 
							<h3>Vishant nimesh<br> 
							<span>Kolkata, India</span> 
							</h3> 
						</div> 
						<div> 
							<span class="dot"> 
								<i class="fas fa-ellipsis-h"></i> 
							</span> 
						</div> 
					</div> 
					<div class="imgBx"> 
						<img src= 
"https://th.bing.com/th/id/OIP.IV7HI0fOER-7KuLdYKyWXQHaGW?pid=ImgDet&w=839&h=720&rs=1"
							alt="post-1"
							class="cover"> 
					</div> 
					<div class="bottom"> 
						<div class="actionBtns"> 
							<div class="left"> 
								<span class="heart"
									onclick="addlike()"> 
									<span> 
										<svg aria-label="Like"
											color="#262626"
											fill="#262626"
											height="24"
											role="img"
											viewBox="0 0 48 48"
											width="24"> 
											<path
												d="M34.6 6.1c5.7 0 10.4 5.2 10.4 
												11.5 0 6.8-5.9 11-11.5 16S25 41.3 
												24 41.9c-1.1-.7-4.7-4-9.5-8.3-5.7-5-11.5-9.2-11.5-16C3 
												11.3 7.7 6.1 13.4 6.1c4.2 0 6.5 2 8.1 
												4.3 1.9 2.6 2.2 3.9 2.5 3.9.3 0 .6-1.3 
												2.5-3.9 1.6-2.3 3.9-4.3 8.1-4.3m0-3c-4.5 
												0-7.9 1.8-10.6 5.6-2.7-3.7-6.1-5.5-10.6-5.5C6 
												3.1 0 9.6 0 17.6c0 7.3 5.4 12 10.6 16.5.6.5 
												1.3 1.1 1.9 1.7l2.3 2c4.4 3.9 6.6 5.9 7.6 
												6.5.5.3 1.1.5 1.6.5.6 0 1.1-.2 1.6-.5 1-.6 
												2.8-2.2 7.8-6.8l2-1.8c.7-.6 1.3-1.2 2-1.7C42.7 
												29.6 48 25 48 17.6c0-8-6-14.5-13.4-14.5z"> 
											</path> 
										</svg> 
									</span> 
								</span> 
								<svg aria-label="Comment"
									class="_8-yf5 "
									color="#262626"
									fill="#262626"
									height="24"
									role="img"
									viewBox="0 0 48 48"
									width="24"> 
									<path clip-rule="evenodd"
										d="M47.5 46.1l-2.8-11c1.8-3.3 2.8-7.1 
										2.8-11.1C47.5 11 37 .5 24 .5S.5 11 .5 24 11 
										47.5 24 47.5c4 0 7.8-1 11.1-2.8l11 2.8c.8.2 
										1.6-.6 1.4-1.4zm-3-22.1c0 4-1 7-2.6 10-.2.4-.3.9-.2 
										1.4l2.1 8.4-8.3-2.1c-.5-.1-1-.1-1.4.2-1.8 
										1-5.2 2.6-10 2.6-11.4 0-20.6-9.2-20.6-20.5S12.7 
										3.5 24 3.5 44.5 12.7 44.5 24z" 
										fill-rule="evenodd"> 
								</path> 
								</svg> 
								<svg aria-label="Share Post"
									class="_8-yf5 "
									color="#262626"
									fill="#262626"
									height="24"
									role="img"
									viewBox="0 0 48 48"
									width="24"> 
									<path
										d="M47.8 3.8c-.3-.5-.8-.8-1.3-.8h-45C.9 
										3.1.3 3.5.1 4S0 5.2.4 5.7l15.9 15.6 5.5 
										22.6c.1.6.6 1 1.2 1.1h.2c.5 0 1-.3 
										1.3-.7l23.2-39c.4-.4.4-1 .1-1.5zM5.2 
										6.1h35.5L18 18.7 5.2 6.1zm18.7 
										33.6l-4.4-18.4L42.4 8.6 23.9 39.7z"> 
									</path> 
								</svg> 
							</div> 
							<div class="right"> 
								<svg aria-label="Save"
									class="_8-yf5 "
									color="#262626"
									fill="#262626"
									height="24"
									role="img"
									viewBox="0 0 48 48"
									width="24"> 
									<path
										d="M43.5 48c-.4 0-.8-.2-1.1-.4L24 29 5.6 
										47.6c-.4.4-1.1.6-1.6.3-.6-.2-1-.8-1-1.4v-45C3 .7 
										3.7 0 4.5 0h39c.8 0 1.5.7 1.5 1.5v45c0 .6-.4 
										1.2-.9 1.4-.2.1-.4.1-.6.1zM24 26c.8 0 
										1.6.3 2.2.9l15.8 16V3H6v39.9l15.8-16c.6-.6 
										1.4-.9 2.2-.9z"> 
									</path> 
								</svg> 
							</div> 
						</div> 
						<a href="#"> 
							<p class="likes">184 likes</p> 
						</a> 
						<a href="#"> 
							<p class="message"> 
							<b>Mayank</b> Nature 
								<span>#love</span> 
								<span>#2021</span> 
							</p> 
						</a> 
						<a href="#"> 
							<h4 class="comments">View all 25 comments</h4> 
						</a> 
						<a href="#"> 
							<h5 class="postTime">9 hours ago</h5> 
						</a> 
						<div class="addComments"> 
							<div class="reaction"> 
								<h3> 
								<i class="far fa-smile"></i> 
							</h3> 
							</div> 
							<input type="text"
								class="text"
								placeholder="Add a comment..."> 
							<a href="#">Post</a> 
						</div> 
					</div> 
				</div> 
			</div> 
			<div class="col-3"> 
				<div class="card"> 
					<h4>Suggestions For You</h4> 
					<div class="top"> 
						<div class="userDetails"> 
							<div class="profilepic"> 
								<div class="profile_img"> 
									<div class="image"> 
										<img src= 
"2.jpg"
											alt="img12"> 
									</div> 
								</div> 
							</div> 
							<h3>Aditya Verma<br> 
							<span>Follows You</span> 
							</h3> 
						</div> 
						<div> 
							<a href="#"
							class="follow">follow 
							</a> 
						</div> 
					</div> 
					<div class="top"> 
						<div class="userDetails"> 
							<div class="profilepic"> 
								<div class="profile_img"> 
									<div class="image"> 
										<img src= 
"1.jpg"
											alt="img13"> 
									</div> 
								</div> 
							</div> 
							<h3>Amit Singh<br> 
							<span>Follows You</span> 
						</h3> 
						</div> 
						<div> 
							<a href="#"
							class="follow">follow 
						</a> 
						</div> 
					</div> 
					<div class="top"> 
						<div class="userDetails"> 
							<div class="profilepic"> 
								<div class="profile_img"> 
									<div class="image"> 
										<img src= 
"3.jpg"
											alt="img14"> 
									</div> 
								</div> 
							</div> 
							<h3>Piyush Agarwal<br> 
								<span>Followed by Keshav Agarwal</span> 
							</h3> 
						</div> 
						<div> 
							<a href="#"
							class="follow">follow</a> 
						</div> 
					</div> 
					<div class="top"> 
						<div class="userDetails"> 
							<div class="profilepic"> 
								<div class="profile_img"> 
									<div class="image"> 
										<img src= 
"4.jpg"
											alt="img15"> 
									</div> 
								</div> 
							</div> 
							<h3>Amirnder singh<br> 
							<span>Follows You</span> 
							</h3> 
						</div> 
						<div> 
							<a href="#"
							class="follow">follow 
						</a> 
						</div> 
					</div> 
					<div class="top"> 
						<div class="userDetails"> 
							<div class="profilepic"> 
								<div class="profile_img"> 
									<div class="image"> 
										<img src= 
"5.jpg"
											alt="img16"
											class="cover"> 
									</div> 
								</div> 
							</div> 
							<h3>Raj Goel<br> 
								<span>Followed by Keshav Agarwal</span> 
							</h3> 
						</div> 
						<div> 
							<a href="#"
							class="follow">follow 
							</a> 
						</div> 
					</div> 
				</div> 
				
			<!-- Our Footer Section will start from Here -->
				<div class="footer"> 
					<a class="footer-section" href="#">About</a> 
					<a class="footer-section" href="#">Help</a> 
					<a class="footer-section" href="#">API</a> 
					<a class="footer-section" href="#">Jobs</a> 
					<a class="footer-section" href="#">Privacy</a> 
					<a class="footer-section" href="#">Terms</a> 
					<a class="footer-section" href="#">Locations</a> 
					<br> 
					<a class="footer-section" href="#">Top Accounts</a> 
					<a class="footer-section" href="#">Hashtag</a> 
					<a class="footer-section" href="#">Language</a> 
					<br><br> 
					<span class="footer-section"> 
						© 2023 INSTAGRAM FROM FACEBOOK 
					</span> 
				</div> 
			</div> 
		</div> 
	</main> 
</body> 
</html>
