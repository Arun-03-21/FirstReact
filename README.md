This is a simple React application that demonstrates the use of useState and useEffect hooks. The app has two counters, "First" and "Second", each with buttons to increment or decrement their values. The useEffect hook is used to simulate data fetching on initial component mount.

Features
State Management: Uses the useState hook to manage two independent counter states.
Effect Hook: Implements the useEffect hook to simulate data fetching on component mount.
User Interaction: Provides buttons to increment and decrement the counter values.
Project Structure
graphql
Copy code
React Counter Application
├── public
│   └── index.html         # The main HTML file
├── src
│   ├── App.js             # Main App component
│   └── index.js           # Entry point for the React application
├── package.json           # Project dependencies and scripts
└── README.md              # Project documentation
Getting Started
Prerequisites
Before running this application, make sure you have the following installed:

Node.js (version 12 or later)
npm (Node package manager, comes with Node.js)
Installation
Clone the Repository:

bash
Copy code
git clone https://github.com/your-username/react-counter-app.git
Navigate to the Project Directory:

bash
Copy code
cd react-counter-app
Install Dependencies:

bash
Copy code
npm install
Running the Application
Start the Development Server:

bash
Copy code
npm run dev
This command will start the development server using Vite and the application will be accessible at http://localhost:5173.

Build the Application: To build the application for production, run:

bash
Copy code
npm run build
Preview the Production Build: To preview the production build locally, run:

bash
Copy code
npm run preview
Usage
Open the application in your browser at http://localhost:5173.
You will see two counters, "First" and "Second", displayed on the screen.
Click on the ADD First button to increment the value of the "First" counter by 1.
Click on the ADD Second button to decrement the value of the "Second" counter by 1.
The useEffect hook will trigger the getData function, logging "Data Received" to the console when the component mounts.
Code Explanation
State Management:

jsx
Copy code
const [first, setFirst] = useState(1);
const [second, setSecond] = useState(100);
first and second represent two separate pieces of state, initialized to 1 and 100 respectively.
setFirst and setSecond are functions used to update their corresponding state values.
Effect Hook:

jsx
Copy code
useEffect(() => {
  getData();
}, []);
The useEffect hook calls getData() once when the component mounts, simulating a data fetch.
Event Handlers:

The ADD First button increments the first state by 1.
The ADD Second button decrements the second state by 1.
Dependencies
React: A JavaScript library for building user interfaces.
Vite: A fast build tool that leverages native ES modules for development and optimizes for production.
