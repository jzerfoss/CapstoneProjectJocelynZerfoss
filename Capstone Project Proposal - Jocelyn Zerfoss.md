**Travel Planner Application \- Capstone Project Proposal**   
**Description** 

The Travel Planning Assistant Web App aims to simplify the trip planning process by providing tailored recommendations for flights, hotels, destinations, and activities. By using real-time data from multiple APIs, this application will enable users to plan their trips more efficiently and within budget. With features like dynamic itinerary generation, weather forecasting, and personalized recommendations, the app will be a comprehensive platform for travelers.

1. **Stack Focus**   
   This project will be a full-stack application with an even distribution of focus between both the front-end and back-end. The goal is to provide a feature-rich web app with a strong back-end to manage API interactions, user data, and dynamic content. At the same time, the front-end will need to be intuitive, interactive, and responsive to enhance the user experience. The back-end will handle user authentication, store data, and make real-time API calls to fetch relevant travel information, while the front-end will display this data in an easy-to-understand manner.

**Front-End:**

* **React.js**: React will be used for building dynamic, responsive, and interactive user interfaces. The component-based architecture will allow for easier scaling of the application as additional features are added.  
* **CSS/SCSS**: For styling the application with custom themes and responsive layouts to ensure accessibility across all devices.

**Back-End:**

* **Node.js**: For handling the server-side logic, making API requests, and managing server operations.  
* **Express.js**: A web framework for building RESTful APIs that will interact with external services and the PostgreSQL database.  
* **PostgreSQL**: A relational database management system (RDBMS) for storing structured data related to users, trips, preferences, and other application information.  
* **JWT (JSON Web Tokens)**: For user authentication and session management.  
* **Amadeus API**: For flight, hotel, and destination data.  
* **OpenWeatherMap API**: For real-time weather data to suggest optimal travel dates.  
* **Yelp API**: For user reviews and suggestions for activities and attractions.

2. **Type**   
   The project will be developed as a web application. Given the nature of the project, targeting users on various devices and browsers is crucial. A responsive design will ensure that the app works seamlessly on both desktop and mobile platforms. 

3. **Goal** 

The goal of this project is to provide users with a personalized travel planning experience by offering tailored recommendations based on real-time data from multiple APIs. The app will serve as a comprehensive platform for users to plan their trips by:

* Suggesting the best flight and hotel options based on user preferences and budget.  
* Providing a dynamic itinerary generator that adapts to the user’s interests.  
* Offering weather forecasts and activity recommendations for various destinations.  
* Helping users stay within their travel budget by suggesting cost-effective options.  
4. **Users** 

The app is designed for travelers of all ages, particularly those who are looking to plan trips more efficiently. The target demographic includes:

* Young professionals (aged 25-40) who are tech-savvy and frequently travel for both work and leisure.  
* Families looking for vacation destinations and activities tailored to their interests and budgets.  
* Solo travelers and adventure seekers who want to explore new destinations.  
* Frequent travelers who need to streamline their travel planning and budgeting process.  
5. **Data** 

To provide dynamic travel recommendations, the app will integrate several external APIs:

* **Amadeus Travel API**: For real-time flight, hotel, and destination data.  
* **OpenWeatherMap API**: For weather forecasts at various destinations.  
* **Yelp API**: For reviews and recommendations on activities, restaurants, and attractions.  
* **Google Maps API**: To provide destination visualizations and help users plan routes.  
* **Public Event APIs**: For fetching local events and activities.

These external APIs will allow the app to provide users with up-to-date travel information that is relevant to their trip planning.

6. **Other Relevant Information**

	**A. Database Schema and Structure**

Since PostgreSQL is a relational database, the data will be stored in structured tables. Below is an overview of the tables and their relationships:

1\. Users Table

Stores information about users, their preferences, and authentication details.

2\. Trips Table

Stores details of each trip that a user has planned or saved.

3\. Activities Table

Stores details about activities in various destinations.

4\. Weather Table

Stores weather data for different destinations at different times.

5\. Flights Table

Stores available flight details from Amadeus API.

6\. Hotels Table

Stores available hotel options, including price and ratings.

**B. API Considerations**

* **Data Quality and Normalization**: Data from external APIs will need to be cleaned and normalized before storing it in the database. This will involve standardizing units (e.g., currencies and temperatures) and ensuring that the data structure is consistent.  
* **API Rate Limits**: To prevent hitting rate limits from third-party APIs, the app will use caching strategies to store previously fetched results and reduce the number of calls made.  
* **Error Handling**: Proper error handling will be required to manage issues with external API failures or rate limiting.