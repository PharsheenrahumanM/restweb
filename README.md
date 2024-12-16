# Ex.07 Restaurant Website
## Date:16/12/2024

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```

home.html
<!DOCTYPE html>

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="resthome.jpg" rel="stylesheet">
    <title>FaRz RESTAURANT</title>
    <style>
        body {
            margin: 0;
            font-family: 'Merienda', cursive;
            background: url('resthome.jpg') no-repeat center center fixed;
            background-size: cover;
            color: rgb(234, 245, 16);
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }

        header {
            text-align: center;
            padding: 50px 20px;
            background: rgba(0, 0, 0, 0.5);
            border-bottom: 2px solid goldenrod;
        }

        header h1 {
            font-size: 80px;
            letter-spacing: 10px;
            margin: 0;
            text-shadow: 2px 2px 8px black;
        }

        nav {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background: rgba(0, 0, 0, 0.7); 
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.5);
            z-index: 1000;
        }

        nav ul {
            list-style: none;
            margin: 0;
            padding: 10px 20px;
            display: flex;
            justify-content: center;
        }

        nav li {
            margin: 0 20px;
        }

        nav a {
            text-decoration: none;
            color:azure;
            font-size: 18px;
            font-weight: 600;
            padding: 10px 20px;
            border-radius: 5px;
        }

        

        main {
            flex: 1;
            padding: 40px;
            text-align: center;
            background: rgba(255, 255, 255, 0.1); 
            margin: 20px auto;
            max-width: 900px;
            border-radius: 15px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.7);
            animation: fadeInUp 1.5s ease-in-out;
        }

        main p {
            font-size: 24px;
            font-weight: 400;
            line-height: 1.5;
            color:yellow;
            text-shadow: 1px 1px 3px black;
        }

        footer {
            background: rgba(0, 0, 0, 0.8); 
            color: white;
            text-align: center;
            padding: 20px 0;
            border-top: 2px solid greenyellow;
            box-shadow: 0 -4px 6px rgba(0, 0, 0, 0.5);
        }

        footer p {
            margin: 5px 0;
            font-size: 16px;
        }

        footer a {
            color: goldenrod;
            text-decoration: none;
            margin: 0 10px;
            font-size: 18px;
            transition: color 0.3s ease-in-out;
        }

        footer a:hover {
            color: #d4af37;
        }

       
    </style>
</head>
<body>
    <header>
        <h1>FaRz RESTAURANT!!!!!</h1>
    </header>
    <nav>
        <ul>
            <li><a href="#" title="Home">Home</a></li>
            <li><a href="menu.html" title="menu">menu</a></li>
            <li><a href="admin.html" title="adminis">Administration</a></li>
            <li><a href="contact.html" title="Contact Us">Contact</a></li>
        </ul>
    </nav>
    <main>
        <p>Welcome to FaRz Restaurant </p>
        <p>Family Restaurant</p>
    </main>
    <footer>
        <p>&copy; 2023 FaRz Restaurant | Designed by: <b>PharsheenRahuman M</b></p>
        <p>
            <a href="#" title="Facebook">Facebook</a> |
             |
            <a href="#" title="Instagram">Instagram</a>
        </p>
    </footer>
</body>
</html>
food.html

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial initial-scale=1.0">
    <title>GRAND - Menu</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500&family=Playfair+Display:wght@700&display=swap"
        rel="stylesheet">
    <style>
        /* General Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background: linear-gradient(to bottom, #e0eafc, #cfdef3);
            line-height: 1.6;
            color: #333;
        }

        /* Header */
        header {
            background: linear-gradient(to right, #4facfe, #00f2fe);
            color: white;
            padding: 15px 30px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        header h1 {
            font-family: 'Playfair Display', serif;
            font-size: 1.8rem;
        }

        header nav a {
            text-decoration: none;
            color: white;
            font-weight: 500;
            margin: 0 15px;
            transition: color 0.3s ease, transform 0.2s ease;
        }

        header nav a:hover {
            color: #ff9800;
            transform: translateY(-2px);
        }

        /* Main Menu Section */
        .menu-container {
            padding: 50px 20px;
            text-align: center;
        }

        .menu-container h1 {
            font-size: 2.7rem;
            color: #333;
            font-family: 'Playfair Display', serif;
            margin-bottom: 20px;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.1);
        }

        .menu-items {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            padding: 20px 10px;
        }

        .menu-item {
            background: white;
            border-radius: 12px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .menu-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            transition: transform 0.3s ease;
        }

        .menu-item:hover {
            transform: scale(1.1);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }

        .menu-item:hover img {
            transform: scale(1.15);
        }

        .menu-details {
            padding: 10px 15px;
            text-align: left;
        }

        .menu-details h3 {
            font-size: 1.2rem;
            color: #555;
            font-weight: 600;
            margin-bottom: 5px;
        }

        .menu-details p {
            font-size: 0.9rem;
            color: #666;
        }

        .menu-details .price {
            color: #e74c3c;
            font-weight: bold;
            margin-top: 5px;
        }

        /* Footer */
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 15px 0;
            font-size: 0.9rem;
        }

        footer a {
            color: #ff9800;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #f4f4f4;
        }

        /* Media Queries */
        @media (max-width: 768px) {
            header h1 {
                font-size: 1.6rem;
            }

            .menu-items {
                grid-template-columns: 1fr 1fr;
            }
        }

        @media (max-width: 480px) {
            .menu-container h1 {
                font-size: 2rem;
            }

            .menu-items {
                grid-template-columns: 1fr;
            }

            .menu-item img {
                height: 180px;
            }
        }
    </style>
</head>

<body>
    <!-- Header Section -->
    <header>
        <h1>Grand</h1>
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="admin.html">Admin</a>
        </nav>
    </header>

    <!-- Main Menu Section -->
    <div class="menu-container">
        <h1>FaRzFoOdS</h1>
        <div class="menu-items">
            <div class="menu-item">
                <img src="biryani.jpeg" alt="Classic Briyani">
                <div class="menu-details">
                    <h3>Classic Briyani</h3>
                    <p class="price">₹399/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="chapati.jpeg" alt="chapati">
                <div class="menu-details">
                    <h3>chappati</h3>
                    <p class="price">₹120/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="dosa.jpeg" alt="dosaa">
                <div class="menu-details">
                    <h3>Dosa</h3>
                    <p class="price">₹70/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="fish.jpeg" alt="fish">
                <div class="menu-details">
                    <h3>Fish</h3>
                    <p class="price">₹250/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="idly.jpeg" alt="idly">
                <div class="menu-details">
                    <h3>Idly</h3>
                    <p class="price">₹120/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="noodles.jpeg" alt="noodles">
                <div class="menu-details">
                    <h3>noodles</h3>
                    <p class="price">₹300/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="poori.jpeg" alt="poori">
                <div class="menu-details">
                    <h3>Poori</h3>
                    <p class="price">₹100/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="prawn.jpeg" alt="prawn">
                <div class="menu-details">
                    <h3>prawn</h3>
                    <p class="price">₹300/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="ramen.jpeg" alt="ramen">
                <div class="menu-details">
                    <h3>ramen</h3>
                    <p class="price">₹100/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="parotta.jpeg" alt="parotta">
                <div class="menu-details">
                    <h3>Parotta</h3>
                    <p class="price">₹75/-</p>
                </div>
            </div>

        </div>
    </div>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2024 GRAND | <a href="#">Back to Home</a></p>
    </footer>
</body>

</html>

admin.html

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chefs</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Caveat:wght@700&family=Pacifico&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            background-color:yellow;
        }

        header {
            text-align: center;
            background-color: #0e6ff5;
            padding: 20px 0;
        }

        header h1 {
            font-family: "Caveat", cursive;
            font-size: 50px;
            color: white;
            margin: 0;
        }


        .chefs-container {
            display: flex;
            gap: 20px;
            padding: 40px;
            margin: auto;
        }

        .chef-card {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            text-align: center;
        }

        .chef-card:hover {
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }

        .chef-card img {
            width: 100%;
            object-fit: contain; 
            max-height: 300px; 
        }

        .chef-details {
            padding: 20px;
        }

        .chef-details h1 {
            font-size: 20px;
            color: rgb(181, 101, 29);
            margin: 10px 0;
        }

        .chef-details h2,
        .chef-details h3 {
            font-size: 16px;
            color: rgb(85, 85, 85);
            margin: 5px 0;
        }

       
        footer {
            text-align: center;
            background-color:aliceblue;
            color:brown;
            padding: 10px 0;
            margin-top: 20px;
        }

        footer p {
            margin: 0;
        }
    </style>
</head>
<body>

  
    <header>
        <h1>Cooking chef</h1>
    </header>

    
    <div class="chefs-container">
        <div class="chef-card">
            <img src="me.jpg" alt="PharsheenRahuman">
            <div class="chef-details">
                <h1>PharsheenRahuman</h1>
                <h2>CEO</h2>
                
            </div>
        </div>
        
        <div class="chef-card">
            <img src="manish.jpeg" alt="Manish Mehrotra">
            <div class="chef-details">
                <h1>Manish Mehrotra</h1>
                <h2>Designation: Executive Chef</h2>
                <h3>Experience: 7 years</h3>
            </div>
        </div>
        <div class="chef-card">
            <img src="sanjeev.jpeg" alt="Sanjeev Kapoor">
            <div class="chef-details">
                <h1>Sanjeev Kapoor</h1>
                <h2>Designation: celebrity Chef</h2>
                <h3>Experience: 2 years</h3>
            </div>
        </div>
        <div class="chef-card">
            <img src="vikaskhanna.jpeg" alt="Vikas Khanna">
            <div class="chef-details">
                <h1>Vikas Khanna</h1>
                <h2>Designation: Michelin Star Chef, Restaurateur, Author</h2>
                <h3>Experience: 5 years</h3>
            </div>
        </div>
        <div class="chef-card">
            <img src="ranveerbrar.jpeg" alt="Ranveerbrar">
            <div class="chef-details">
                <h1>Miss Cheruba</h1>
                <h2>Designation:Celebrity Chef, Restaurateur, Television Host</h2>
                <h3>Experience: 3 years</h3>
            </div>
        </div>
        
       
    <footer>
        <p>&copy; 2024 Foodie's Paradise. All rights reserved.</p>
    </footer>

</body>
</html>
contact.html
<html>
    <head>
        <link rel="preconnect" href="https://fonts.googleapis.com">
        <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
        <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400..700&display=swap" rel="stylesheet">
        <title>Contact Us</title>
        <style>
            #n1{
                position: relative;
                color:navy;
                font-size: 60px;
                padding-left: 380px;
                left: 0px;
                top: 190px;
                letter-spacing: 5px;
            }
            body{
                background-image: url("resthome.jpg");
                background-repeat: no-repeat;
                background-size: 1700px 950px;
            }
            #n2{
                position:relative;
                color: gray;
                font-size: 80px;
                padding-left: 480px;
                top: 140px;
                letter-spacing: 3px;
                font-family: "Dancing Script", cursive;
            }
            #n3{
                position: relative;
                color: gray;
                font-size: 35px;
                top: 255px;
                padding-left: 240px;
            }
            #n4{
                position: relative;
                color:darkmagenta;
                font-size:31px;
                top: 205px;
                padding-left: 170px;
                letter-spacing: 2px;
            }
            #n5{
                position: relative;
                color: aliceblue;
                font-size: 35px;
                top: 60px;
                padding-left: 680px;
            }
            #n6{
                position: relative;
                color:crimson;
                font-size:35px;
                top: 8px;
                padding-left: 505px;
            }
            #n7{
                position: relative;
                color: aliceblue;
                font-size: 35px;
                bottom: 135px;
                padding-left: 1155px;
            }
            #n8{
                position: relative;
                color:darksalmon;
                font-size: 31px;
                bottom: 187px;
                padding-left: 950px;
                text-align: center;
            }

           
            a {
                color:red;
                text-decoration: none;
                cursor: pointer;
            }

      
            a:hover {
                text-decoration: underline;
            }
            
        </style>
    </head>
    <body>
        <h1 id="n1">Welcome</h1>
        <h2 id="n2">Quality and Taste</h2>
        <h5 id="n3">Phone:</h5>
        <h5 id="n4">
            <a href="tel:+919669966969">+91 6546456456</a>
        </h5>
        <h5 id="n5">Email:</h5>
        <h5 id="n6">
            <a href="mailto:farz101@gmail.com"><b>farz101@gmail.com</b></a>
        </h5>
        <h5 id="n7">Location:</h5>
        <h5 id="n8">
            <a href="FaRz restarurant"><b> FaRz restaurant in chennai-600 035</b></a>
        </h5>
    </body>
</html>



```
## OUTPUT:
![homerest](https://github.com/user-attachments/assets/e25fe394-32d9-4465-8441-2a17b181b8b5)

![7menu](https://github.com/user-attachments/assets/2c11ec64-5d62-4094-a773-6edbd5fc23f4)

![7chefs](https://github.com/user-attachments/assets/e3ddbb00-ef27-4338-be58-8c21f169a093)

![contrest](https://github.com/user-attachments/assets/f1ab54a9-7aa9-4492-a073-122dce7f4584)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
