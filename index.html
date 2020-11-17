<!DOCTYPE html>
<html>
    
<head>
   <title> Sign Up Page</title> 
    <link rel="stylesheet" href="css/style.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    
</head>    
 <body>
<h1>Welcome to the Sign Up Page</h1>
<br><br>
<div id = "mainContent">
<form id="signupForm" action="welcome.html">
    First Name: <input type="text" name="fName"><br>
    Last Name:  <input type="text" name="lName"><br>
    Gender:     <input type="radio" name="gender" value="m"> Male
                <input type="radio" name="gender" value="f">Female<br>      
    Zip Code:   <input type="text" id="zip" name="zip"><br>
                <span id="zipError"></span><br>
    City:       <span id="city"></span><br>
    Latitude:   <span id="latitude"></span><br>

    Longitude:  <span id="longitude"></span><br>

    
    State: <select id="state" name="state"></select><br>
 
    Select a County:  <select id="county"></select><br>
    Desired Username: <input type="text" id="username" name="username"><br>
                       <span id="usernameError"></span><br>
    Password:         <input type="password" id="password" name"password"><br>
                    
    Password Again:   <input type="password" id="passwordAgain"><br>
                       <span id="passwordAgainError"></span ><br /><br>
 
 

 
 
         <input type="submit" value="Sign up!">
         </form>
         
        </div> 
         
    <footer>
    <hr>
            
        CST336: Internet Programming Lab 3. 2020&copy; Randolph
            
    </footer>
 
 <script>
    var usernameAvailable = false;
    //fills in options for states using api 
    async function populateStates(){
        let url = `https://cst336.herokuapp.com/projects/api/state_abbrAPI.php`;
        let response = await fetch(url);
        let data = await response.json();
      
        $("#state").html(`<option> Select A State </option>`);
        for(let i = 0; i < data.length; i++){
            $("#state").append(`<option value="${data[i].usps}"> ${data[i].state} </option>`);
        }
    }
    
    //displaying City from API after typing a zip code
    $("#zip").on("change", async function(){
      isValid = true;
      //alert($("#zip").val());
      let zipCode = $("#zip").val();
      
      let url =  `https://itcdland.csumb.edu/~milara/ajax/cityInfoByZip?zip=${zipCode}`;
      let response = await fetch(url);
      let data = await response.json();
      
      if(data){
       $("#city").html(data.city);
       $("#latitude").html(data.latitude);
       $("#longitude").html(data.longitude);
       $("#zipError").html("Valid").css("color", "green");  
      }
      else{
            $("#city").html("");
            $("#latitude").html("");
            $("#longitude").html("");
            $("#zipError").html("Zip Code not found.").css("color", "red");
      }
      console.log(data);
      
    });//zip
    
    populateStates();
    
    $("#state").on("change", async function(){
    //alert($("#state").val()); 
    let state = $("#state").val();
    let url = `https://cst336.herokuapp.com/projects/api/countyListAPI.php?state=${state}`;
    let response = await fetch(url);
    let data = await response.json();
    //console.log(data);   
    
    $("#county").html(`<option> Select A County </option>`);
    for(let i=0; i < data.length; i++) {
        $("#county").append(`<option> ${data[i].county} </option>`);
    }
        
    });//state
    
     $("#username").on("change", async function(){
        //alert($("#username").val());
        let username = $("#username").val();
      let url = `https://cst336.herokuapp.com/projects/api/usernamesAPI.php?username=${username}`;
      let response = await fetch(url);
      let data = await response.json();
      
      if (data.available) {
        $("#usernameError").html("Username available!");
        $("#usernameError").css("color", "green");
        usernameAvailable = true;
    
      }
      else {
          $("#usernameError").html("Username not available!");
          $("#usernameError").css("color", "red"); 
          usernameAvailable = false;
       }
    });//username
    
    $("#signupForm").on("submit", function(e){
        //alert("Submitting form...");
        if(!isFormValid()){
        e.preventDefault();
        }
    });
    
   function isFormValid(){
        isValid = true;
        if(!usernameAvailable){
            isValid = false;
        }
       
       if($("#username").val().length == 0){
           isValid = false;
           $("#usernameError").html("Username is required").css("color", "red");
       }
       
       
       if ($("#password").val() != $("#passwordAgain").val())
       {
           $("#passwordAgainError").html("Password Mismatch!").css("color", "red");;
            isValid = false;
       }
       
       else if($("#password").val().length < 6)
       {
            $("#passwordAgainError").html("Password must be at least 6 characters!").css("color", "red");;
            isValid = false;
       }

      return isValid;  
    }

 </script>
 </body>   
</html>