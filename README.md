<!DOCTYPE html>
<html>
    <head>
        <title>Restaurant Website</title>
        <style>
            html{
                scroll-behavior: smooth;
            }
            body{
                margin: 0;
                padding: 0;
                font-size: 16px;
                font-family: Arial, Helvetica, sans-serif;
                cursor: pointer;
                background:lightgray;
            }
            header h1{
                margin: 0;
                padding: 0;
                height:200px;
                padding: 10px;
                display: flex;
                justify-content: center;
                align-items: center;
                color: #ff5733;
                background:black;
                font-size:50px;
                font-weight: bolder;
                box-sizing: border-box;
            }
            #navigation-links{
                background: #ff5733;
                height: 50px;
                margin-top:-27px;
                font-size:20px;
                font-weight: bold;
            }
            .links{
                display: flex;
                justify-content:space-around;
            }
            .links a{
                padding: 13px 20px;
                color: black;
                list-style: none;
                text-decoration: none;
                transition: transform 0.2s ease-in-out ,0.2s ease-in-out;
            }
            .links a:hover{
                color: #ff5733;
                background:black;
                transform: scale(1.02);
            }
            #welcome-section h1{
                display: flex;
                align-items: center;
                justify-content: center;
            }

            #about{
                color: black;
                background:#ff8a6f;
                height:220px;
                margin: 0 5%;
                border: 5px solid black;
                border-radius: 30px;
                transition: transform 0.3s ease-in-out ,0.3s ease-in-out;
            }
            #about:hover{
                transform: scale(1.02);
            }
            #about-p{
                padding:20px;
                letter-spacing:2px;
                font-size:18px;
                box-sizing: border-box;
            }
            @media (max-width:1286px){
                #about{
                    height: 240px;
                }
            }
            @media (max-width:1102px) {
                #about-p{
                    font-size:14px;
                }
                
            }
            @media (max-width:546px){
                #about-p{
                    background: #000;
                }
            }
            #menu h1{
                display: flex;
                align-items: center;
                justify-content: center;
            }
            #menu table{
                width:90%;
                height: auto;
                margin: 0 5%;
                border-collapse:collapse;
                font-size:19px;
                transition:transform 0.3s ease-in-out;
                letter-spacing: 2px;
            }
            table:hover{
                transform: scale(1.02);
            }
            th{
                color: #ff5733;
                background:rgb(0, 0, 0);
                font-size: 22px;
            }
            td{
                color: black;
                background:#ff6e4d;
                font-weight: bold;
            }
            th , td{
                width: 100px;
                height:85px;
                border: 1px solid black;
                text-align:center;
                vertical-align:middle;
                padding: 10px;
            }
            td img{
                width:200px;
                height:auto; 
                display: block;
                margin: auto;
                object-fit: cover;
            }
            #menu table th{
                font-size:20px;
            }

            #contact-container{
                display: flex;
                align-items: center;
                justify-content: center;
                margin-top: 20px;
                padding: 20px;
                background:linear-gradient(black,#ff5733);
                transition:transform 0.3s ease-in-out;
            }
            #contact-container:hover{
                transform: scale(1.02);
            }
            #contact{
                display: flex;
                flex-direction:column;
                width: 320px;
                background:white;
                padding: 20px;
                border-radius: 20px;
                box-shadow:  0 0 10px rgba(0, 0, 0, 0.1);
            }
            #contact h1{
                color: #ff5733;
                font-weight: bold;
                display: flex;
                align-items: center;
                justify-content: center;
            }
            form{
                display: flex;
                flex-direction: column;
            }
            label{
                font-weight: bold;
            }
            input , textarea{
                margin:10px 0;
            }
            textarea{
                resize: none;
                height:80px;
            }
            button{
                color: #000;
                background: #ff5733;
                padding:8px;
                border: 0;
                border-radius: 30px;
                width:100px;
                font-size:17px;
                font-weight: bold;
                margin-top: 10px;
                margin-left:30%;
            }
            button:hover {
                background: #ff2f01;
                transform: scale(1.05);
            }
            footer{
                margin-top: 20px;
                color:#ff5733;
                background: #000;
                height:50px;
                font-size: 18px;
                text-align: center;
                padding:10px;
                letter-spacing: 2px;
                transition:transform 0.3s ease-in-out;
            }
            footer:hover{
                transform: scale(1.02);
            }

            
        </style>
    </head>
    <body>
        <header>
            <div id="home">
                <h1>Delcious Bites</h1>
            </div>

            <div id="navigation-links">
                <div class="links">
                    <a href="#home">Home</a>
                    <a href="#about">About</a>
                    <a href="#menu">Menu</a>
                    <a href="#contact">Contact</a>
                </div>
            </div>
        </header>

        <main>
            <div id="welcome-section">
                <h1>Welcome To Our Restaurant</h1>
            </div>

            <div id="about">
                <div id="about-p">
                    Welcome to Our Restaurant , where delicious flavors meet a warm and inviting atmosphere. We take
                    pride in serving fresh, high-quality ingredients crafted into mouthwatering dishes that satisfy every
                    craving. Whether you're here for a casual meal, family gathering, or a special occasion, our team is
                    dedicated to providing you with an exceptional dining experience.
                    <br>
                    At Our Restaurant , we believe in the perfect balance of taste, tradition, and innovation. Our
                    chefs carefully curate each dish, blending classic recipes with modern twists to bring you a memorable 
                    culinary journey. From sizzling appetizers to decadent desserts, every bite is a celebration of flavor.
                    <br>
                    Come and experience great food, a cozy ambiance, and top-notch hospitality—we can’t wait to serve you! 🍽️✨
                </div>
            </div>

            <div id="menu">
                <h1>Restaurant Menu</h1>

            <table>
                <tr>
                    <th>Dishes</th>
                    <th>Description</th>
                    <th>Prices</th>
                    <th>Images</th>
                </tr>
                <tr>
                    <td>Margherita Pizza</td>
                    <td>Classic cheese and tomato pizza</td>
                    <td>$12.99</td>
                    <td><img src="imagess/PIZZA.jpg" alt=""></td>
                </tr>
                <tr>

                    <td>Grilled Chicken</td>
                    <td>Served with fresh vegetables</td>
                    <td>$15.99</td>
                    <td><img src="imagess/GRILLED CHICKEN.webp" alt=""></td>
                </tr>
                <tr>
                    <td>Pasta Alfredo</td>
                    <td>Rich and creamy sauce with fettuccine</td>
                    <td>$14.49</td>
                    <td><img src="imagess/ALFREDO PASTA.webp" alt=""></td>
                </tr>
                <tr>
                    <td>Chocolate Cake</td>
                    <td>Delicious homemade chocolate cake</td>
                    <td>$6.99</td>
                    <td><img src="imagess/CHOCOLATE CAKE (1).webp" alt=""></td>
                </tr>
            </table>
            </div>
            
            <div id="contact-container">
            
            <div id="contact">
                <h1>Contact Us</h1>
                <form action="">
                    <label for="name">Name</label>
                    <input type="text" name="name" required>

                    <label for="email">Email</label>
                    <input type="email" name="email" required>

                    <label for="message">Message</label>
                    <textarea name="message" id="message"></textarea>

                    <button type="submit">Submit</button>
                </form> 
            </div>
        </div>
        </main>

        <footer>
            <p>© 2025 Syed Sahil. All rights reserved.</p>
        </footer>
    </body>
</html>
