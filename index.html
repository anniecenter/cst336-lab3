<!DOCTYPE html>
<html>

<head>
    <title>Sign Up Page</title>
    <link href="./styles.css" rel="stylesheet" type="text/css" />
    <!-- Import JQuery Library -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
</head>

<body class="indexBody">
    <div class="spacer"></div>
    <div class="box">
        <h2>Sign Up</h2>
        <form id="signUpForm" action="welcome.html">
            <table>
                <tr>
                    <td>First Name:</td>
                    <td><input type="text" name="fname"><br> </td>
                </tr>
                <tr>
                    <td>Last Name:</td>
                    <td><input type="text" name="lname"><br></td>
                </tr>
                <tr>
                    <td>Gender:</td>
                    <td><input type="radio" name="gender" value="m"> Female<input type="radio" name="gender" value="f"> Male</td>
                </tr>
                <tr>
                    <td></td>
                    <td><br></td>
                </tr>
                <tr>
                    <td>Zip Code:</td>
                    <td><input type="text" id="zip" name="zip"></td>
                </tr>
                <tr>
                    <td>City:</td>
                    <td><span id="city"></span></td>
                </tr>
                <tr>
                    <td>Latitude:</td>
                    <td><span id="lat"></span></td>
                </tr>
                <tr>
                    <td>Longitude:</td>
                    <td><span id="long"></td>
                </tr>
                <tr>
                    <td>State:</td>
                    <td>
                        <select id="state" name="state">
                            <option>Select One</option>
                            <option value="ca">California</option>
                            <option value="ny">New York</option>
                            <option value="tx">Texas</option>
                        </select>
                    </td>
                </tr>
                <tr>
                    <td>Select a County:</td>
                    <td><select id="county"></select></td>
                </tr>
                <tr>
                    <td></td>
                    <td><br></td>
                </tr>
                <tr>
                    <td>Desired Username:</td>
                    <td><input type="text" id="username" name="username"></td>
                    <td><span id="usernameError"></span></td>
                </tr>
                <tr>
                    <td>Password:</td>
                    <td><input type="password" id="password" name="password"></td>
                    <td><span id="passwordError"></span></td>
                </tr>
                <tr>
                    <td>Confirm Password:</td>
                    <td><input type="password" id="confirmPassword" name="confirmPassword"></td>
                    <td><span id="confirmPasswordError"></span></td>
                </tr>
                <tr>
                    <td></td>
                    <td><br></td>
                </tr>
                <tr>
                    <td><input type="submit" value="Sign up!"></td>
                </tr>
            </table>
            
        </form>
    </div>
    <div class="spacer"></div>

    <script>
        var usernameAvailable = false;

        // Displaying City from API after typing a zip code
        $("#zip").on("change", async function() {
            //alert($("#zip").val());
            let zipCode = $("#zip").val();
            let url = `https://itcdland.csumb.edu/~milara/ajax/cityInfoByZip.php?zip=${zipCode}`;
            let response = await fetch(url);
            let data = await response.json();
            //console.log(data);
            $("#city").html(data.city);
            $("#lat").html(data.latitude);
            $("#long").html(data.longitude);
        }); // zip

        $("#state").on("change", async function() {
            //alert($("#state").val());
            let state = $("#state").val();
            let url = `https://itcdland.csumb.edu/~milara/ajax/countyList.php?state=${state}`;
            let response = await fetch(url);
            let data = await response.json();
            //console.log(data);
            $("#county").html("<option>Select One</option>");
            for (let i = 0; i < data.length; i++) {
                $("#county").append(`<option>${data[i].county}</option>`);
            }
        }); // state

        $("#username").on("change", async function() {
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
        }); // username

        $("#signUpForm").on("submit", function(e) {
            //alert("Submitting form...");
            if (!isFormValid()) {
                e.preventDefault();
            }
        }); // sign-up form

        function isFormValid() {
            isValid = true;
            if (!usernameAvailable) {
                isValid = false;
            }

            if ($("#username").val().length == 0) {
                isValid = false;
                $("#usernameError").html("Username is required");
                $("#usernameError").css("color", "red");
            }

            if ($("#password").val().length < 6) {
                $("#passwordError").html("Password must have at least 6 characters");
                $("#passwordError").css("color", "red");
                isValid = false;
            }

            if ($("#password").val() != $("#confirmPassword").val()) {
                $("#confirmPasswordError").html("Passwords do not match");
                $("#confirmPasswordError").css("color", "red");
                isValid = false;
            }

            return isValid;
        }
    </script>
</body>

</html>
