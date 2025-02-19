# User Management System

## Description
The **User Management System** is a simple RESTful API built using Node.js without any external frameworks like Express.js. It allows users to be managed through a JSON file, enabling operations such as retrieving, adding, and deleting users.

## Features
- **GET /users**: Retrieve all users stored in a JSON file.
- **POST /users**: Accept new user data and add it to the JSON file.
- **DELETE /users/:id**: Remove a user by their ID from the JSON file.
- Uses asynchronous file system operations for efficient data handling.

## Technologies Used
- **Node.js**
- **http module**
- **fs (File System) module**
- **path module**

## Installation
1. Ensure you have [Node.js](https://nodejs.org/) installed on your system.
2. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/user-management-system.git
   ```
3. Navigate to the project directory:
   ```sh
   cd user-management-system
   ```
4. Install dependencies (if required in future updates):
   ```sh
   npm install
   ```

## Usage
1. Open a terminal and navigate to the project directory.
2. Start the server using:
   ```sh
   node server.js
   ```
3. The server will start at `http://localhost:3000`.
4. Use **Postman** to interact with the following endpoints:
   
   - **GET /users**
     - Open Postman and create a new request.
     - Set the request type to `GET`.
     - Enter the URL: `http://localhost:3000/users`.
     - Click `Send` to retrieve all users.
   
   - **POST /users**
     - Open Postman and create a new request.
     - Set the request type to `POST`.
     - Enter the URL: `http://localhost:3000/users`.
     - Go to the `Body` tab and select `raw`, then choose `JSON` format.
     - Enter the following JSON data:
       ```json
       {
         "name": "John Doe",
         "email": "john@example.com"
       }
       ```
     - Click `Send` to add the user.
   
   - **DELETE /users/:id**
     - Open Postman and create a new request.
     - Set the request type to `DELETE`.
     - Enter the URL: `http://localhost:3000/users/{id}` (replace `{id}` with an actual user ID).
     - Click `Send` to delete the user.

## Example JSON File (users.json)
```json
[
  {
    "id": "1712345678901",
    "name": "John Doe",
    "email": "john@example.com"
  }
]
```

## Contributing
Feel free to fork this repository and submit pull requests with improvements.

## Author
[Vrushank Ganatra](https://github.com/MerLin027)
