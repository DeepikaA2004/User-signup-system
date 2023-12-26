# User Signup System

This PHP script is a simple user signup system that allows users to create an account with a unique username and password. It uses a MySQL database to store user information securely.

## Prerequisites

Before running this script, ensure that you have the following:

- PHP installed on your server.
- MySQL database set up with the required configuration.
- Bootstrap CSS included for styling (already included in the code).

## Setup

1. **Clone the repository to your local machine or download the PHP file (`signup.php`) directly.**

    ```bash
    git clone https://github.com/yourusername/your-repository.git
    ```

2. **Configure the database connection by updating the `dbconnect.php` file with your database credentials.**

    ```php
    // dbconnect.php

    $server = "your-server";
    $username = "your-username";
    $password = "your-password";
    $database = "your-database";

    $conn = mysqli_connect($server, $username, $password, $database);

    if (!$conn) {
        die("Connection failed: " . mysqli_connect_error());
    }
    ```

3. **Import the SQL schema provided in the `users.sql` file to create the necessary 'users' table in your database.**

    ```bash
    mysql -u your-username -p your-database < users.sql
    ```

4. **Run the PHP script by navigating to the project directory in your browser or using a local server.**

    ```bash
    php -S localhost:8000
    ```

    Visit `http://localhost:8000/signup.php` in your browser to access the signup form.

## Usage

- Open the signup form in your browser.
- Enter a unique username, password, and confirm the password.
- Click the "SignUp" button to create a new account.
- Success and error messages will be displayed based on the signup outcome.

## Contributing

Feel free to contribute to the improvement of this user signup system. Create a fork, make your changes, and submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
