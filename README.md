# Ex04 Places Around Me
# Date:27-10-2024
# AIM
To develop a website to display details about the places around my house.

# DESIGN STEPS
## STEP 1
Create a Django admin interface.

## STEP 2
Download your city map from Google.

## STEP 3
Using <map> tag name the map.

## STEP 4
Create clickable regions in the image using <area> tag.

## STEP 5
Write HTML programs for all the regions identified.

## STEP 6
Execute the programs and publish them.

# CODE

map.html
~~~
<html>
    <head>
        <title> My City</title>
    </head>
    <body>
        <h1 align="center">
            <font color="red">
                <b>Teynampet</b>
            </font>
        </h1>
        <h3 align="center">
            <font color="blue">
                <b>
                    Naveen Kumar E (24006129)
                </b>
            </font>
        </h3>
        <center>
            <img src="Screenshot 2024-12-06 183016.png" usemap="#MyCity" height="610" width="1450">
            <map name="MyCity">
                <area shape="circle" coords="1307,558'25" title="visit kauvery hospital" href="kauvery.html" >
                <area shape="circle" coords="933,340,19" title="visit hyatt Regency" href="hyatt.html" >
                <area shape="circle" coords="780,768,15" title="visit apollo hospital" href="apollo.html" >
                <area shape="rect" coords="587,478,713,509" title="vist titan" href="titan.html">
                <area shape="circle" coords="1300,221,15" title="visit itc hotel" href="itc.html" >
            </map>
        </center>
    </body>
</html>
~~~

hyatt.html

~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hyatt Regency</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f7f7f7;
        }
        header {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px;
        }
        header h1 {
            margin: 0;
            font-size: 2.5em;
        }
        header p {
            margin: 5px 0 0;
            font-size: 1.2em;
            color: #d4af37;
        }
        .container {
            padding: 20px;
            text-align: center;
        }
        .container h2 {
            font-size: 2em;
            color: #444;
        }
        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }
        .gallery img {
            width: 300px;
            height: 200px;
            object-fit: cover;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease;
        }
        .gallery img:hover {
            transform: scale(1.05);
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            margin-top: 20px;
        }
        footer p {
            margin: 0;
            font-size: 0.9em;
            color: #d4af37;
        }
    </style>
</head>
<body>
    <header>
        <h1>Hyatt Regency</h1>
        <p>Luxury and Comfort Redefined</p>
    </header>
    <div class="container">
        <h2>Explore Our Stunning Spaces</h2>
        <p>Experience the unparalleled luxury of the Hyatt Regency. Here’s a glimpse of our beautiful facilities:</p>
        <div class="gallery">
            <img src="waiting hall.jpg" alt="Hyatt Regency Lobby">
            <img src="rooms.webp" alt="Luxury Suite">
            <img src="swimming pool.jpg" alt="Swimming Pool">
            <img src="dining area.webp" alt="Dining Area">
            <img src="event hall.avif" alt="Event Hall">
            <img src="Outdoor Garden.webp" alt="Outdoor Garden">
        </div>
    </div>
    <footer>
        <p>&copy; 2024 Hyatt Regency | All Rights Reserved</p>
    </footer>
</body>
</html>
~~~

kauvery.html

~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kauvery Hospital</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #0077b6;
            color: white;
            padding: 20px;
            text-align: center;
        }
        .container {
            padding: 20px;
        }
        .gallery {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            justify-content: center;
        }
        .gallery img {
            width: 300px;
            height: 200px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s;
        }
        .gallery img:hover {
            transform: scale(1.05);
        }
        footer {
            background-color: #0077b6;
            color: white;
            text-align: center;
            padding: 10px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Kauvery Hospital</h1>
        <p>Your Health, Our Priority</p>
    </header>
    <div class="container">
        <h2>Our Facilities</h2>
        <p>Kauvery Hospital is dedicated to providing the best healthcare services. Here are some glimpses of our facilities:</p>
        <div class="gallery">
            <img src="k hospital front.avif" alt="Hospital Building">
            <img src="Patient Care Unit.jpeg" alt="Patient Care Unit">
            <img src="Advanced Equipment.webp" alt="Advanced Equipment">
            <img src="Emergency Department.jpeg" alt="Emergency Department">
            <img src="waiting area h.jpeg" alt="Waiting Area">
            <img src="Operation Theater.webp" alt="Operation Theater">
        </div>
    </div>
    <footer>
        <p>&copy; 2024 Kauvery Hospital | All Rights Reserved</p>
    </footer>
</body>
</html>

~~~

itc.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ITC Hotels</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
        }
        header {
            background-color: #013220;
            color: white;
            text-align: center;
            padding: 20px;
        }
        header h1 {
            margin: 0;
            font-size: 2.5em;
        }
        header p {
            margin: 5px 0 0;
            font-size: 1.2em;
            color: #f0a500;
        }
        .container {
            padding: 20px;
            text-align: center;
        }
        .container h2 {
            font-size: 2em;
            color: #333;
        }
        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }
        .gallery img {
            width: 300px;
            height: 200px;
            object-fit: cover;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease;
        }
        .gallery img:hover {
            transform: scale(1.05);
        }
        footer {
            background-color: #013220;
            color: white;
            text-align: center;
            padding: 10px;
            margin-top: 20px;
        }
        footer p {
            margin: 0;
            font-size: 0.9em;
            color: #f0a500;
        }
    </style>
</head>
<body>
    <header>
        <h1>ITC Hotel</h1>
        <p>Luxury Redefined with Sustainable Hospitality</p>
    </header>
    <div class="container">
        <h2>Explore Our World-Class Facilities</h2>
        <p>Experience luxury, elegance, and comfort at ITC Hotels. Here's a glimpse of what we offer:</p>
        <div class="gallery">
            <img src="ITC Grand Entrance.jpg" alt="ITC Grand Entrance">
            <img src="Luxury Suites.avif" alt="Luxury Suites">
            <img src="Fine Dining Restaurant.jpg" alt="Fine Dining Restaurant">
            <img src="Wellness Spa.png" alt="Wellness Spa">
            <img src="Conference Hal.jpeg" alt="Conference Hall">
            <img src="swimming-pool itc.jpg" alt="Poolside View">
        </div>
    </div>
    <footer>
        <p>&copy; 2024 ITC Hotels | All Rights Reserved</p>
    </footer>
</body>
</html>

~~~
apollo.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Apollo Hospital</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
        }
        header {
            background-color: #002f6c;
            color: white;
            text-align: center;
            padding: 20px 0;
        }
        header h1 {
            margin: 0;
            font-size: 2.5em;
        }
        header p {
            margin: 5px 0;
            font-size: 1.2em;
        }
        .container {
            padding: 20px;
            text-align: center;
        }
        .container h2 {
            font-size: 2em;
            color: #333;
        }
        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }
        .gallery img {
            width: 300px;
            height: 200px;
            object-fit: cover;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease;
        }
        .gallery img:hover {
            transform: scale(1.05);
        }
        footer {
            background-color: #002f6c;
            color: white;
            text-align: center;
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
        <h1>Apollo Hospital</h1>
        <p>Exceptional Healthcare, Trusted Everywhere</p>
    </header>
    <div class="container">
        <h2>Our World-Class Facilities</h2>
        <p>Explore some of the modern facilities and patient care amenities at Apollo Hospital:</p>
        <div class="gallery">
            <img src="front.jpg" alt="Apollo Hospital Front View">
            <img src="apollo-hospital-panchavati-nashik-private-hospitals-zzfhlk71fz.avif" alt="Patient Rooms">
            <img src="dr-sivaraman-p-b-apollo-hospitals--greames-road-chennai-urologist-doctors-ywmra.avif" alt="Diagnostic Center">
            <img src="professional-medical-with-new-technologies-hospital-ward-modern-emergency-room_116317-24458.avif" alt="Emergency Ward">
            <img src="maxresdefault.jpg" alt="Pharmacy">
            <img src="Screen Shot 2021-10-01 at 11.23.10 AM.jpg" alt="Advanced Surgical Equipment">
        </div>
    </div>
    <footer>
        <p>&copy; 2024 Apollo Hospital | All Rights Reserved</p>
    </footer>
</body>
</html>

~~~

titan.html

~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Titan Brand</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9;
        }
        header {
            background-color: #1a1a1a;
            color: white;
            text-align: center;
            padding: 20px;
        }
        header h1 {
            margin: 0;
            font-size: 2.5em;
        }
        header p {
            margin: 10px 0 0;
            font-size: 1.2em;
            color: #ffcc00;
        }
        .container {
            padding: 20px;
            text-align: center;
        }
        .container h2 {
            font-size: 2em;
            color: #333;
        }
        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }
        .gallery img {
            width: 250px;
            height: 250px;
            object-fit: cover;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease;
        }
        .gallery img:hover {
            transform: scale(1.05);
        }
        footer {
            background-color: #1a1a1a;
            color: white;
            text-align: center;
            padding: 10px;
            margin-top: 20px;
        }
        footer p {
            margin: 0;
            font-size: 0.9em;
            color: #ffcc00;
        }
    </style>
</head>
<body>
    <header>
        <h1>Titan</h1>
        <p>Timeless Elegance, Crafted for You</p>
    </header>
    <div class="container">
        <h2>Our Iconic Collections</h2>
        <p>Discover the artistry and sophistication of Titan’s watches, jewelry, and accessories:</p>
        <div class="gallery">
            <img src="watch collection.jpg" alt="Titan Watches - Classic Collection">
            <img src="raga watch.webp" alt="Titan Raga - Women’s Watches">
            <img src="edge watch.webp" alt="Titan Edge - Ultra Slim Watches">
            <img src="gold titan.jpg" alt="Titan Jewelry Collection">
            <img src="glasses.jpg" alt="Titan Eye Plus - Eyewear">
            <img src="smart watch.jpg" alt="Titan Smartwatches">
        </div>
    </div>
    <footer>
        <p>&copy; 2024 Titan Company Limited | All Rights Reserved</p>
    </footer>
</body>
</html>

~~~
# OUTPUT
Map
![Screenshot 2024-12-06 221102](https://github.com/user-attachments/assets/f631fc5d-bf5f-4b7d-8ca9-794900aad090)

Hyatt
![Screenshot 2024-12-06 221041](https://github.com/user-attachments/assets/baf07371-fe1a-44c5-9d47-ebd98755bd7f)

Kauvery
![Screenshot 2024-12-06 221148](https://github.com/user-attachments/assets/e67472d0-f8e5-4da1-8158-a67cbf24a3a6)

ITC hotel
![Screenshot 2024-12-06 221315](https://github.com/user-attachments/assets/d98b2658-f8de-483d-aebc-86fafe055074)

Apollo
![Screenshot 2024-12-06 221007](https://github.com/user-attachments/assets/6fbf6a29-a9f8-4e0a-aac8-d97ec1ea705f)

Titan
![Screenshot 2024-12-06 221245](https://github.com/user-attachments/assets/3552b452-9fc0-4dcf-8a79-a367a7ff2d3e)



# RESULT
The program for implementing image maps using HTML is executed successfully.
