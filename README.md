# CODTECH-Task2
TASK2 - WEATHER APP USING HTML,CSS AND JAVASCRIPT

![Screenshot 2024-07-18 203133](https://github.com/user-attachments/assets/b38d20d5-5d25-4ff9-82f8-a6bdb5022ccf)
![Screenshot 2024-07-18 212116](https://github.com/user-attachments/assets/98247213-507b-48ca-a5dc-f5798424725b)




NAME : JENIFER Y
COMPANY: CODTECH IT SOLUTIONS
DOMAIN: WEB DEVELOPMENT
ID: CT4W2714
MENTOR: MUZZAMIL

OVERVIEW OF MY PROJECT:

key activities:
1. **Responsive Styling**: Defines responsive layout and visual theme using CSS, including gradient backgrounds and Flexbox for alignment.

2. **User Interaction**: Implements interactive elements like search input and button, enhancing usability and accessibility.

3. **API Integration**: Connects to OpenWeather API via JavaScript to fetch and display real-time weather data based on user input.

4. **Error Handling**: Manages error messages for invalid city names, ensuring clear feedback to users while maintaining UI integrity.
HTML Structure:
Search Section: Contains an input field for entering a city name and a button with a search icon.
Error Message Section: Initially hidden, displays an error message if the city entered is invalid.
Weather Display Section: Initially displays weather information for New York as placeholder.
Weather Icon: Initially shows a rain icon (rain.png).
Temperature: Displayed in Celsius (22°C).
City Name: Initially set to New York.
Details: Displays humidity and wind speed information.
JavaScript:
API Configuration: Defines apiKey and apiUrl for accessing OpenWeatherMap API.
DOM Element References: Retrieves references to HTML elements using querySelector.
checkWeather Function: Asynchronously fetches weather data for the specified city:
Handles 404 error if city is not found.
Updates DOM elements with weather information if city is found.
Updates weather icon based on weather condition using a switch statement.
Event Listener: Listens for clicks on the search button and calls checkWeather with the value entered in the search input field.


* { ... }: This sets default styles for all elements on the page:

margin: 0; padding: 0;: Removes default margin and padding from all elements.
font-family: 'Poppins', 'sans-serif';: Sets the font family to 'Poppins' or a generic sans-serif font.
box-sizing: border-box;: Ensures padding and border are included in the element's total width and height.
body { ... }: Styles applied directly to the <body> element:

background-color: #222;: Sets the background color of the entire page to a dark grayish-blue (#222).
.card { ... }: Styles for the main container .card that holds the weather app content:

width: 90%; max-width: 450px;: Sets the width to 90% of the parent container or a maximum of 450px.
background: linear-gradient(220deg, #00246B, #CADCFC);: Applies a linear gradient background from a dark blue (#00246B) to a light blue (#CADCFC).
color: aliceblue;: Sets the text color to a light blueish-white (aliceblue).
margin: 100px auto 0;: Centers the .card horizontally (auto for left and right margins) and positions it 100px from the top.
border-radius: 25px;: Rounds the corners of the .card with a border radius of 25px.
padding: 35px 40px;: Adds internal padding of 35px on top and bottom, and 40px on left and right sides.
text-align: center;: Centers the text content inside the .card.
.search { ... }: Styles for the search bar section within .card:

width: 100%;: Makes the search bar span the entire width of its container.
display: flex; align-items: center; justify-content: space-between;: Uses Flexbox to align items horizontally with space between them.
.search input { ... }: Styles for the input field within .search:

border: 0; outline: 0;: Removes border and outline.
background: #ebfffc;: Sets a light greenish background color for the input field.
color: #555;: Sets the text color to a dark gray (#555).
padding: 10px 25px;: Adds internal padding of 10px top and bottom, and 25px left and right.
height: 60px;: Sets the height of the input field to 60px.
border-radius: 30px;: Rounds the corners of the input field with a border radius of 30px.
flex: 1; margin-right: 16px;: Makes the input field flexible to fill available space, with margin on the right.
.search button { ... }: Styles for the search button within .search:

border: 0; outline: 0;: Removes border and outline.
background: #ebfffc;: Sets a light greenish background color for the button.
border-radius: 50%;: Rounds the button into a circle with a border radius of 50%.
width: 60px; height: 60px;: Sets the dimensions of the button to 60px by 60px.
cursor: pointer;: Changes the cursor to a pointer when hovering over the button.
.search button img { ... }: Styles for the search icon image within the search button:

width: 16px;: Sets the width of the search icon image to 16px.
.weather-icon { ... }: Styles for the weather icon image:

width: 170px;: Sets the width of the weather icon image to 170px.
margin-top: 30px;: Adds margin of 30px on top of the weather icon image.

.weather h1, .weather h2 { ... }: Styles for <h1> and <h2> elements within .weather:
font-size: 80px; font-weight: 500;: Sets the font size to 80px for <h1> and 45px for <h2>, with respective font weights.

.error { ... }: Styles for the error message section:
text-align: left; margin-left: 10px;: Aligns text to the left with left margin of 10px.
font-size: 25px; margin-top: 10px;: Sets font size to 25px and adds margin of 10px from the top.
display: none;: Initially hides the error message section.
