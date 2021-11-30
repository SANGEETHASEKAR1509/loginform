<html> 

    <head> 

        <script> 

            function GEEKFORGEEKS() { 

                var name =  

                    document.forms["RegForm"]["Name"]; 

                var email =  

                    document.forms["RegForm"]["EMail"]; 

                var phone =  

                    document.forms["RegForm"]["Telephone"]; 

                var what =  

                    document.forms["RegForm"]["Subject"]; 

                var password =  

                    document.forms["RegForm"]["Password"]; 

                var address =  

                    document.forms["RegForm"]["Address"]; 

  

                if (name.value == "") { 

                    window.alert("Please enter your name."); 

                    name.focus(); 

                    return false; 

                } 

  

                if (age.value == "") { 

                    window.alert("Please enter your age."); 

                    address.focus(); 

                    return false; 

                } 

  

                if (email.value == "") { 

                    window.alert( 

                      "Please enter a valid e-mail address."); 

                    email.focus(); 

                    return false; 

                } 

  

                if (phone.value == "") { 

                    window.alert( 

                      "Please enter your telephone number."); 

                    phone.focus(); 

                    return false; 

                } 

  

                if (password.value == "") { 

                    window.alert("Please enter your password"); 

                    password.focus(); 

                    return false; 

                } 

  

                if (what.selectedIndex < 1) { 

                    alert("Please enter your course."); 

                    what.focus(); 

                    return false; 

                } 

  

                return true; 

            } 

        </script> 

  

        <style> 

            div { 

                box-sizing: border-box; 

                width: 100%; 

                border: 100px solid black; 

                float: left; 

                align-content: center; 

                align-items: center; 

            } 

  

            form { 

                margin: 0 auto; 
                padding: 24px;
                width: 600px; 
                background-color: aqua;
                align-content: center;

            } 

        </style> 

    </head> 

  

    <body style="background-color:lightgray;"> 

        

        <form name="RegForm" action="/submit.php" 

              onsubmit="return GEEKFORGEEKS()" method="post"> 
              <h1 style="text-align: center;">REGISTRATION FORM</h1> 

            <p><b>NAME: </b><br><input type="text" 

                            size="50" name="Name" /></p> 

            <p><b>AGE: </b><br> <input type="text" 

                               size="50" name="Address" /> 

          </p> 

          <p><b>E-MAIL ADDRESS: </b><br><input type="text" 

                            size="50" name="EMail" /></p> 


            <p><b>PASSWORD:</b> <br><input type="password" 

                         size="50" name="Password" /></p> 


            <p><b>TELEPHONE:</b> <br><input type="text" 

                        size="50" name="Telephone" /></p> 

  

            <p> 

                <b>SELECT YOUR COURSE </b>

                <select type="text" value="" name="Subject"> 

                    <option>BTECH</option> 

                    <option>BBA</option> 

                    <option>BCA</option> 

                    <option>B.COM</option> 

                    <option>GEEKFORGEEKS</option> 

                </select> 

            </p> 

                <input type="submit" 

                       value="Login" name="Submit" /> 

                <input type="reset" 

                       value="Reset" name="Reset" /> 

            </p> 

        </form> 

    </body> 

</html> 






