# BloggerReview
<html>
  <head>
    <title>
      Blogger Review
    </title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap" rel="stylesheet">
    <style>
      html {
        background-color:#facadc;
        justify-content:center;
        align-item : center;
        display: flex;
      }
      body {
        width: 90%;
        border-radius: 20px;
        background-color:#faf0f4;
        margin-top: 50px;
      }
      .header {
        justify-content:center;
        align-item : center;
        display: flex;
      }
      .header h1 {
        font-family: "Poppins", sans-serif;
        font-weight:bold;
        font-style: normal;
      }
      .navBar {
        display : flex;
      }
      .navBar ul {
        list-style-type: none;
        display:flex;
        gap:30px;
        position : relative;
        top:5px;
      }
      .navBar ul li a:active {
        background-color: black;
        color: white;
        border-radius:12px;
      }
      .navBar ul li a {
        text-decoration: none;
        color : black;
        font-family: "PT Sans", sans-serif;
        font-weight: bold;
        font-style: normal;
        padding : 10px;
      }
      .navBar .searchIcon {
        width:250px;
        position: relative;
        right: -570px;
        top:5px;
        padding : 0px 10px;
        border-radius:30px;
        background-color:#fcebf2;
        display:flex;
        border:3px solid #ff0066;
        cursor : pointer;
      }
      .navBar .searchIcon img {
        height : 20px;
        width  : 20px;
        padding : 10px;
        border-radius: 50%;
        background-color : #f2bdd2;
        position: relative;
        top: 4px;
        left:-4.5px;
      }
      .navBar .searchIcon input[type="search"] {
        width: 200px;
        padding: 5px;
        outline : none;
        border : none;
        background-color : rgba(0,0,0,0);
      }
      input::placeholder {
        color: gray;
        font-size: 16px;
        font-weight: bold;
        padding : 5px;
        font-family: "Poppins", sans-serif;
        font-weight:bold;
        font-style: normal;
      }
      form {
        font-family: "Poppins", sans-serif;
        padding: 20px;
        width : 600px;
        justify-content:center;
        align-item : center;
        display : grid;
      }
      form input, form textarea {
        width: 100%;
        padding: 10px;
        margin: 10px 0;
        border: 1px solid #ccc;
        border-radius: 5px;
        font-size: 16px;
      }
      form input[type="submit"] {
        background-color: #ff0066;
        color: white;
        border: none;
        cursor: pointer;
      }
      form input[type="submit"]:hover {
        background-color: #cc0055;
      }
    </style>
  </head>
  <body>
    <div class="navBar">
      <ul>
        <li><a href="#">HOME</a></li>
        <li><a href="#">BLOG</a></li>
        <li><a href="#">SETTINGS</a></li>
        <li><a href="#">CONTACT ME</a></li>
      </ul>
      <div class="searchIcon">
        <img src="https://static-00.iconduck.com/assets.00/search-icon-2044x2048-psdrpqwp.png">
        <input type="search" placeholder="Type to search...">
      </div>
    </div>
    <hr>
    <div class="header">
      <h1>Your Opinion matters</h1>
    </div>
    <form action="/submit-review" method="post">
      <label for="name">Name:</label>
      <input type="text" id="name" name="name" placeholder="Enter your name" required>

      <label for="dob">Date of Birth:</label>
      <input type="date" id="dob" name="dob" required>

      <label for="address">Address:</label>
      <input type="text" id="address" name="address" placeholder="Enter your address" required>

      <label for="mobile">Mobile Number:</label>
      <input type="tel" id="mobile" name="mobile" placeholder="Enter your mobile number" required>

      <label for="email">Email ID:</label>
      <input type="email" id="email" name="email" placeholder="Enter your email" required>

      <label for="review">Review:</label>
      <textarea id="review" name="review" rows="4" placeholder="Share your review..." required></textarea>

      <label for="suggestions">Any suggestions?</label>
      <textarea id="suggestions" name="suggestions" rows="4" placeholder="Any suggestions for improvement?"></textarea>

      <input type="submit" value="Submit Review">
    </form>
  </body>
</html>
