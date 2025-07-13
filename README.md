🎥 ReelFinder
Find the perfect movie for any mood! ReelFinder is an intuitive web application that lets you search for movies and discover what's trending, all powered by the vast TMDB database and a robust backend managed by Appwrite.

✨ Features
Movie Search: Easily find your favorite movies or discover new ones by entering search terms.

Trending Movies: Explore the most popular and trending movies right on the homepage.

Details & Trailers (Coming Soon!): We're working on adding the ability to view detailed movie information and watch trailers directly within the app!

Search Counter: Popular searches are recorded and used to enhance the user experience (e.g., by showing real-time trends).

🛠 Technologies Used
Frontend:

React: For building the interactive and dynamic user interface.

Vite: A fast build tool and development server for modern JavaScript projects.

Tailwind CSS: For rapid and efficient styling.

Backend & Database:

Appwrite: An open-source backend platform that manages the database for search terms and trending movie data.

External API:

The Movie Database (TMDB) API: The primary source for movie data (movie information, posters, etc.).

🚀 Getting Started
Follow these steps to set up and run ReelFinder on your local machine.

Prerequisites
Make sure you have the following installed:

Node.js (version 14 or higher recommended)

npm (usually comes with Node.js) or Yarn

Project Setup
Clone the repository:

Bash

git clone https://github.com/your-username/reelfinder.git
cd reelfinder
Install dependencies:

Bash

npm install
# or if you use yarn
yarn
Appwrite and TMDB Configuration:
ReelFinder uses environment variables for API keys and Appwrite IDs. Create a .env file in the root of your project with the following content:

Code snippet

VITE_TMDB_API_KEY=your_tmdb_api_key
VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id
VITE_APPWRITE_DATABASE_ID=your_appwrite_database_id
VITE_APPWRITE_COLLECTION_ID=your_appwrite_collection_id
VITE_TMDB_API_KEY: Get your free API key from The Movie Database (TMDB).

VITE_APPWRITE_PROJECT_ID, VITE_APPWRITE_DATABASE_ID, VITE_APPWRITE_COLLECTION_ID: You'll obtain these IDs from your Appwrite console.

Create a project in Appwrite.

Create a database.

Within that database, create a collection (e.g., search_terms or movie_trends) with the following attributes:

searchTerm (String)

count (Integer)

movie_id (String)

poster_url (String)

Running the Application
Once you've configured your .env file, you can start the application:

Bash

npm run dev
# or if you use yarn
yarn dev
The application will run at http://localhost:5173 (or another available port).

🤝 Contributing
Contributions are welcome! If you have ideas for improving ReelFinder, feel free to open an issue or submit a pull request.

📄 License
This project is licensed under the MIT License. See the LICENSE file for more details.
