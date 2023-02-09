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

		NEXT: #### 9. Design Sign up page


#### 9. Design Sign up page
        
        Activities

        1. Modified readme file
        modified:   README.md

        2. Design Sign up page
        new file:   assets/css/style.css

        body {
		    font-family: roboto, sans-serif;
		    background-color: #E9EBEE;
		    margin: 0;
		    font-size: 16px;
		}

		a {
		    text-decoration: none;
		}

		li {
		    list-style: none;
		}

		textarea:focus,
		input:focus {
		    outline: none;
		}

		.align-middle {
		    display: flex;
		    justify-content: center;
		    align-items: center;
		}

		.main {
		    font-family: Helvetica, Arial, sans-serif;
		    height: 100vh;
		    width: 100vw;
		    display: flex;
		}

		.left-side {
		    flex-basis: 50%;
		    display: flex;
		    justify-content: center;
		    align-items: center;
		}

		.right-side {
		    flex-basis: 50%;
		}

		.error {
		    color: red;
		    font-size: 18px;
		    margin-top: 33px;
		}

		.sign-up-form {
		    margin-top: 10px;
		}

		.text-field {
		    height: 25px;
		    padding: 5px;
		    border: 1px solid lightgray;
		    border-radius: 5px;
		    font-size: 16px;
		}

		.text-input {
		    height: 25px;
		    padding: 5px;
		    border: 1px solid lightgray;
		    border-radius: 5px;
		    font-size: 16px;
		    margin-top: 0.8rem;
		    width: 70%;
		}

		input:-webkit-autofill,
		input:-webkit-autofill:hover,
		input:-webkit-autofill:focus,
		input:-webkit-autofill:active {
		    -webkit-box-shadow: 0 0 0 30px white inset !important;
		}

		.bday {
		    font-size: 19px;
		    color: #141823;
		    margin: 0.8rem 0 5px 0;
		}

		.select-body {
		    display: inline-block;
		    height: 30px;
		    font-size: 13px;
		    border: 1px solid #bdc7d8;
		    color: #141823;
		    border-radius: 5px;
		}

		.gender-wrap {
		    margin: 10px 0;
		}

		.term {
		    font-size: 12px;
		}

		input.sign-up {
		    background: linear-gradient(#67ae55, #578843);
		    background-color: #69a74e;
		    box-shadow: inset 0 1px 1px #a4e388;
		    border-color: #3b6a22 #3b6e22 #2c5115;
		    padding: 10px 50px;
		    border: 1px solid gray;
		    border-radius: 5px;
		    margin: 14px 0;
		    color: white;
		    font-size: 18px;
		}

		NEXT: #### 10. Create birthday date using javascript


#### 10. Create birthday date using javascript
        
        Activities

        1. Modified readme file
        modified:   README.md

        2. Add plugin
        new file:   assets/js/jquery.js

        3. Connect plugin and Create birthday date using javascript
        modified:   signup.php

                <script src="assets/js/jquery.js"></script>

        <!--BIRTHDAY JAVASCRIPT CODE-->
        <script>
        for (i = new Date().getFullYear(); i > 1900; i--) {
            //    2019,2018, 2017,2016.....1901
            $("#years").append($('<option/>').val(i).html(i));

        }
        for (i = 1; i < 13; i++) {
            $('#months').append($('<option/>').val(i).html(i));
        }
        updateNumberOfDays();

        function updateNumberOfDays() {
            $('#days').html('');
            month = $('#months').val();
            year = $('#years').val();
            days = daysInMonth(month, year);
            for (i = 1; i < days + 1; i++) {
                $('#days').append($('<option/>').val(i).html(i));
            }

        }
        $('#years, #months').on('change', function() {
            updateNumberOfDays();
        })

        function daysInMonth(month, year) {
            return new Date(year, month, 0).getDate();

        }

    	</script>


    	DONE :)

    	NEXT: #### 11. Understanding form submission process


#### 11. Understanding form submission process
        
        Activities

        1. Modified readme file
        modified:   README.md

        2. Theory

        Understanding form submission process

        submit > isset > $first_name > db

        NEXT: #### 12. Connecting site with MYSQL database

        
#### 12. Connecting site with MYSQL database
        
        Activities

        1. Modified readme file
        modified:   README.md

        2. Define db connection
        new file:   connect/DB.php

        <!-- connect/DB.php -->
		<?php

		class DB{

		    private static function connect(){
		        $pdo = new PDO('mysql:host=127.0.0.1; dbname=php_facebook_clone; charset=utf8mb4', 'root', 'root');

		        $pdo->setAttribute(PDO::ATTR_ERRMODE, PDO::ERRMODE_EXCEPTION);
		        return $pdo;
		    }

		    public static function query($query, $params = array()){
		        $statement = self::connect()->prepare($query);
		        $statement->execute($params);

		        if(explode(' ', $query)[0] == 'SELECT'){
		            $data = $statement->fetchAll();
		            return $data;
		        }
		    }
		}
		?>

        3. Connecting site with MYSQL database
        modified:   signup.php

        <?php  

		// Load the db
		require 'connect/DB.php';

		DONE :)

		NEXT: #### 13. Create user database table