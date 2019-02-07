# Database
A mini-framework for database


# Usage
- Return following keyword if no records in database: "none"
- Return "Connection failed: " . $this->conn->connect_error if occure any connection errors to database.

# Start object
$database = new Database('127.0.0.1', 'root', '', 'coins');

# Retrive all data
$data = $database->retriveData("SELECT * FROM table");

# Retrive one row
$data = $database->retriveRow("SELECT * FROM table WHERE id='1'");

# Retrive one value (Just username)
$data = $database->retriveValue("SELECT username FROM table WHERE id='1');

# Execute query
$data = $database->execute("DELETE FROM table WHERE id='2'");
