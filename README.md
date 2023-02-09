## MEMBUAT SOCIAL NETWORK 'CLONE FB' DENGAN PHP & MYSQL

https://github.com/gurnitha/php-facebook-clone

Ini adalah latihan saya membuat social network berdasarkan kursus sy di udemy: 
Build a Social Network in 20 Days from Scratch:PHP+MYSQL, Js  

### SECTION 1: Day 1: Course Intro: Info & Setup


#### 1. Welcome to the course (Same as intro)

		PASS 

#### 2. Download and install XAMPP

		PASS 

#### 3. Download,install and config code editor

		PASS 

#### 4. Create necessary folder

		ing@DESKTOP-5NU2HDJ:/mnt/e/workspace/laragon/www/php_facebook_clone$ tree -L 2
		.
		├── README.md
		├── _docs
		│  ├── Complete+Project+Source+Code
		│  ├── Resource file
		│  ├── TOC
		│  └── facebook.sql
		├── assets
		│  ├── css
		│  ├── image
		│  └── js
		├── connect
		├── core
		│  ├── ajax
		│  ├── classes
		│  └── database
		└── views

#### 5. Membuat Remote Github Repository


### SECTION 2: Day 2: Create Sign Up with mobile or email and necessary file system


#### 5. Complete Project Source code & Resource File

		PASS 

#### 6. Section resources

		PASS 

#### 7. All about the folder structure

		PASS 

#### 8. Create Sign up html structure
        
        Activities

        1. Modified readme file
        modified:   README.md

        2. Create Sign up html structure
        new file:   signup.php

        <!DOCTYPE html>
		<html lang="en">
		   <head>
		      <meta charset="UTF-8">
		      <title>facebook</title>
		      <link rel="stylesheet" href="assets/css/style.css">
		   </head>
		   <body>
		      <div class="header">
		      </div>
		      <div class="main" style="width:100%;">
		         <div class="left-side">
		            <img src="assets/image/facebook%20Signin%20image.png" alt="">
		         </div>
		         <div class="right-side">
		            <div class="error">
		            </div>
		            <h1 style="color:#212121;">Create an account</h1>
		            <div style="color:#212121; font-size:20px">It's free and always will be</div>
		            <form action="sign.php" method="post" name="user-sign-up">
		               <div class="sign-up-form">
		                  <div class="sign-up-name">
		                     <input type="text" name="first-name" id="first-name" class="text-field" placeholder="First Name">
		                     <input type="text" name="last-name" id="last-name" placeholder="Last Name" class="text-field">
		                  </div>
		                  <div class="sign-wrap-mobile">
		                     <input type="text" name="email-mobile" id="up-email" placeholder="Mobile number or email address" class="text-input">
		                  </div>
		                  <div class="sign-up-password">
		                     <input type="password" name="up-password" id="up-password" class="text-input" placeholder="Password">
		                  </div>
		                  <div class="sign-up-birthday">
		                     <div class="bday">Birthday</div>
		                     <div class="form-birthday">
		                        <select name="birth-day" id="days" class="select-body"></select>
		                        <select name="birth-month" id="months" class="select-body"></select>
		                        <select name="birth-year" id="years" class="select-body"></select>
		                     </div>
		                  </div>
		                  <div class="gender-wrap">
		                     <input type="radio" name="gen" id="fem" value="female" class="m0">
		                     <label for="fem" class="gender">Female</label>
		                     <input type="radio" name="gen" id="male" value="male" class="m0">
		                     <label for="male" class="gender">Male</label>
		                  </div>
		                  <div class="term">
		                     By clicking Sign Up, you agree to our terms, Data policy and Cookie policy. You may receive SMS notifications from us and can opt out at any time.
		                  </div>
		                  <input type="submit" value="Sign Up" class="sign-up">
		               </div>
		            </form>
		         </div>
		      </div>
		   </body>
		</html>

		NEXT: Design Sign up page


#### 9. Design Sign up page
