# Ex.07 Restaurant Website
## Date:24-12-2024

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
Homepage

```
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="homepage7.css">
    <title>Bakery Website</title>
</head>
<body>

    <div class="header">
        <div class="logo-container">
            <img src="images/baklogo.png" alt="Bakery Logo" class="logo-img">
            <h2 class="bakery-name">Stellar Crust</h2>
        </div>
    </div>

    <div class="navbar">
        <ul class="nav-links">
            <li><a href="homepage7.html">Home</a></li>
            <li><a href="menulist.html">Menu</a></li>
            <li><a href="booktable.html">Book</a></li>
            <li><a href="contacts.html">Contact</a></li>
            <li><a href="admin.html">Admin</a></li>
        </ul>
    </div>

    <center>
    <div class="image-section">
        <div class="content">
            <h2>Welcome to Stellar Crust Bakery!</h2>
            <p>Freshly baked goods made with love. Enjoy our special offers: Buy 1 Get 1 Free on Croissants, 20% off Cakes this weekend, and Free Coffee with every Pastry!</p>
        </div>
    </div>
    </center>
    <center>
    <div class="card-container">
        
        <div class="card">
            <h3>Menu</h3>
            <img src="images/bakery8.jpeg" alt="Menu">
            <p><b>Explore our diverse menu, featuring everything from fresh croissants to decadent cakes.</b></p>
            <a href="menulist.html"><u>View Full Menu</u></a>
        </div>
    
       
        <div class="card">
            <h3>Book a Table</h3>
            <img src="images/bakery9.jpeg" alt="Book a Table">
            <p><b>Reserve your spot today and enjoy our freshly baked goods in a warm and welcoming environment.</b></p>
            <a href="booktable.html"><u>Book Now</u></a>
        </div>
    
        <div class="card">
            <h3>Opening Hours</h3>
            <img src="images/opening2.jpeg" alt="Opening Hours">
            <p><b>We’re open every day to serve you the best baked goods! Check our schedule for more details.</b></p>
            <a href="#"><u>View Hours</u></a>
        </div>
    </div>
</div>
</center>
<div class="footer">
<div class="logo-section">
    <img src="images/baklogo.png" alt="Bakery Logo">
</div>
<div class="hrline">
    <hr>
    <p><b>Preethi D (24007817)</b></p>
</div>
</body>
</html>
```
```
Homepage - CSS


* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Open Sans', sans-serif;
    background-color:#f8e8cf;  /* Soft beige background */
    color: #5a3d32; /* Earthy dark brown for text */
    line-height: 1.6;
    padding: 0px;
   
}


    .header {
        background-color:#B89C85;
        padding: 5px 0;
        text-align: center;
        margin-bottom: 0px;
        display: flex;
        justify-content: center;
        align-items: center;
      
    }


.logo-container {
    display: flex;
    justify-content: center;
    align-items: center;
}

.logo-img {
    height: 120px;
    width: auto;
    margin-right: 5px;
}

.bakery-name {
    font-size: 50px;
    font-weight: 700;
    color:#3d2a1f; 
    font-family: 'Merriweather', serif; 
    text-transform: uppercase;
    letter-spacing: 2px;
}

.navbar {
    background-color: #3d2a1f; 
    padding: 12px 20px;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%; 
    max-width: 1600px; 
    margin-left: auto; 
    margin-right: auto;
}

.nav-links {
    list-style: none;
    display: flex;
    padding: 0;
    margin: 0;
}

.nav-links li {
    margin-left: 30px;
}

.nav-links a {
    color: #f8e8cf;
    text-decoration: none;
    font-size: 18px;
    font-family: 'Open Sans', sans-serif;
    font-weight: 600;
    transition: all 0.3s ease-in-out;
    padding: 10px 15px;
    border-radius: 5px;
}

.nav-links a:hover {
    color: #c9a555; 
    background-color: #5a3d32; 
    transform: scale(1.1); 
}

.nav-links a.active {
    color: #c9a555; 
    font-weight: 700;
    border-bottom: 2px solid #FFD700; 
}


.image-section {
    width: 85%;
    height: 250px; 
    background-image: url('images/slider5.jpg'); 
    background-size: cover; 
    background-position: center; 
    border-radius: 20px;
    margin-top: 40px;
    display: flex;
    justify-content: center;
    align-items: center;
    border: 4px solid #5A3D32;
    box-shadow: 0 6px 18px rgba(0, 0, 0, 0.3);;
}

.image-section .content {
    text-align: center;
    color: #f1e6d8;
    background-color:rgba(57, 27, 4, 0.6); 
    padding: 20px;
    border-radius: 10px;
    font-size: 20px;
    width: 75%;
    font-family: 'Merriweather', serif;
}

.card-container {
    display: flex;
    justify-content: space-between; 
    gap: 10px; 
    margin: 40px auto;
    padding: 0 20px;
    max-width: 1200px; 
    flex-wrap: wrap; 
}

.card {
    background-color :#B89C85; 
    width: 30%; 
    height: 380px;
    border-radius: 12px; 
    box-shadow: 0 6px 18px rgba(0, 0, 0, 0.2); 
    overflow: hidden;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 20px;
    box-sizing: border-box;
    transition: all 0.3s ease-in-out; 
    border: 3px solid #5a3d32;
}

.card:hover {
    transform: translateY(-5px); 
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.25); 
}

.card img {
    width: 100%;
    height: 150px;
    object-fit: cover;
    border-radius: 10px;
    border: 3px solid #5a3d32;
}

.card h3 {
    font-family: 'Roboto', sans-serif; 
    font-size: 20px;
    color:#5a3d32;
    text-align: center;
    font-weight: 700;
    margin-bottom: 10px;
}

.card p {
    font-family: 'Lora', serif; 
    font-size: 16px;
    color: #5A3D32; 
    text-align: center;
    margin: 10px 0;
    line-height: 1.5;
}

.card a {
    display: block;
    text-align: center;
    font-family: 'Roboto', sans-serif;
    font-size: 16px;
    color:  #6E2B1F;
    text-decoration: none;
    font-weight: 600;
    margin-top: auto;
}

.card a:hover {
    color: #ffffff;
}


.logo-section {
    text-align: center;
    position:absolute;
    left: 150px;
    padding: 10px;
    margin-top: 0px; 
    border: 2px solid #7a4b36;
    background-origin: padding-box;
}

.logo-section img {
    width: auto; 
    height: 100px;
    border-radius: 50%; 
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2); 
    border: #7a4b36;
}
.hrline{
   width: 55%;
   border-top: 2px solid #B89C85;
   position: absolute;
   right:100px;
}
.hrline p{
    position: absolute;
    right: 60px;
    font-size: 20px;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
}


@media (max-width: 768px) {
    .card {
        width: 45%; 
        height: auto; 
    }
}

@media (max-width: 480px) {
    .card {
        width: 90%; 
    }
}


@media (max-width: 768px) {
    .logo-container {
        flex-direction: column;
        margin-top: 30px;
    }

    .logo-img {
        margin-bottom: 15px;
    }

    .nav-links {
        flex-direction: column;
        margin-top: 20px;
    }

    .nav-links li {
        margin-left: 0;
        margin-bottom: 10px;
    }

    .image-section {
        height: 200px;
    }

    .content h2 {
        font-size: 22px;
    }

    .content p {
        font-size: 18px;
    }
}
```

## OUTPUT:
Home page
![Screenshot 2024-12-25 120435](https://github.com/user-attachments/assets/8da1235e-6afc-4cca-99d4-516db4964c7e)
![Screenshot 2024-12-25 120451](https://github.com/user-attachments/assets/d3c5a8a6-ad50-403b-984b-685c4f71d2d8)


menu page
![Screenshot 2024-12-25 120616](https://github.com/user-attachments/assets/e637bf18-f851-4d5d-aa5b-cb6006e2cac9)
![Screenshot 2024-12-25 120629](https://github.com/user-attachments/assets/f0e25a24-73e8-4494-b6e6-1bffce3d7530)


seat booking
![Screenshot 2024-12-25 120727](https://github.com/user-attachments/assets/8c68319e-1137-4b79-80e9-7e475cee7d1b)
![Screenshot 2024-12-25 120735](https://github.com/user-attachments/assets/05887971-292d-44e7-acb0-36f9efc49380)


contacts page
![Screenshot 2024-12-25 120822](https://github.com/user-attachments/assets/e427e5a3-4360-4edc-af25-ff4d06ceea13)
![Screenshot 2024-12-25 120830](https://github.com/user-attachments/assets/e795e770-c1fe-42de-aa99-d9e7d8846d58)

 
Administration page
![Screenshot 2024-12-25 120916](https://github.com/user-attachments/assets/8e9f5196-7469-4f46-95d1-9403e78a74ff)
![Screenshot 2024-12-25 120927](https://github.com/user-attachments/assets/64fdce37-da6a-4392-8648-0d6331adfd10)



## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
