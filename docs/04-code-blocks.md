# Code Blocks and Syntax Highlighting

This document demonstrates various ways to include code in Markdown.

## Inline Code

Use `inline code` for short code snippets: `const x = 42;`

Variables like `userName` and `isValid` are shown inline.

File paths: `/usr/local/bin` and `C:\Windows\System32`

## Fenced Code Blocks

### JavaScript

```javascript
// Function to calculate factorial
function factorial(n) {
  if (n === 0 || n === 1) {
    return 1;
  }
  return n * factorial(n - 1);
}

const result = factorial(5);
console.log(`Factorial of 5 is ${result}`);
```

### Python

```python
# Python class example
class Calculator:
    def __init__(self):
        self.result = 0
    
    def add(self, x, y):
        """Add two numbers"""
        self.result = x + y
        return self.result
    
    def multiply(self, x, y):
        """Multiply two numbers"""
        self.result = x * y
        return self.result

calc = Calculator()
print(f"5 + 3 = {calc.add(5, 3)}")
print(f"5 * 3 = {calc.multiply(5, 3)}")
```

### Java

```java
// Java class example
public class HelloWorld {
    private String message;
    
    public HelloWorld(String message) {
        this.message = message;
    }
    
    public void printMessage() {
        System.out.println(message);
    }
    
    public static void main(String[] args) {
        HelloWorld hello = new HelloWorld("Hello, World!");
        hello.printMessage();
    }
}
```

### C++

```cpp
#include <iostream>
#include <vector>
#include <algorithm>

// Template function to find maximum
template<typename T>
T findMax(const std::vector<T>& vec) {
    return *std::max_element(vec.begin(), vec.end());
}

int main() {
    std::vector<int> numbers = {1, 5, 3, 9, 2};
    std::cout << "Maximum: " << findMax(numbers) << std::endl;
    return 0;
}
```

### C#

```csharp
using System;
using System.Linq;

namespace Example
{
    public class Program
    {
        public static void Main(string[] args)
        {
            var numbers = new[] { 1, 2, 3, 4, 5 };
            var sum = numbers.Sum();
            var average = numbers.Average();
            
            Console.WriteLine($"Sum: {sum}");
            Console.WriteLine($"Average: {average}");
        }
    }
}
```

### Go

```go
package main

import (
    "fmt"
    "time"
)

// Goroutine example
func printMessage(msg string, delay time.Duration) {
    time.Sleep(delay)
    fmt.Println(msg)
}

func main() {
    go printMessage("Hello", 1*time.Second)
    go printMessage("World", 2*time.Second)
    
    time.Sleep(3 * time.Second)
    fmt.Println("Done!")
}
```

### Rust

```rust
// Rust struct and implementation
struct Rectangle {
    width: u32,
    height: u32,
}

impl Rectangle {
    fn area(&self) -> u32 {
        self.width * self.height
    }
    
    fn can_hold(&self, other: &Rectangle) -> bool {
        self.width > other.width && self.height > other.height
    }
}

fn main() {
    let rect1 = Rectangle { width: 30, height: 50 };
    let rect2 = Rectangle { width: 10, height: 40 };
    
    println!("Area: {}", rect1.area());
    println!("Can hold: {}", rect1.can_hold(&rect2));
}
```

### Ruby

```ruby
# Ruby class example
class Person
  attr_accessor :name, :age
  
  def initialize(name, age)
    @name = name
    @age = age
  end
  
  def greet
    puts "Hello, my name is #{@name} and I'm #{@age} years old."
  end
  
  def birthday
    @age += 1
    puts "Happy birthday! You are now #{@age}."
  end
end

person = Person.new("Alice", 30)
person.greet
person.birthday
```

### PHP

```php
<?php
// PHP class example
class Database {
    private $connection;
    private $host = "localhost";
    private $username = "root";
    private $password = "";
    
    public function __construct($database) {
        $this->connection = new mysqli(
            $this->host,
            $this->username,
            $this->password,
            $database
        );
    }
    
    public function query($sql) {
        return $this->connection->query($sql);
    }
    
    public function close() {
        $this->connection->close();
    }
}
?>
```

### TypeScript

```typescript
// TypeScript interface and class
interface User {
  id: number;
  name: string;
  email: string;
  role: 'admin' | 'user' | 'guest';
}

class UserManager {
  private users: User[] = [];
  
  addUser(user: User): void {
    this.users.push(user);
  }
  
  findUserById(id: number): User | undefined {
    return this.users.find(user => user.id === id);
  }
  
  getAdminUsers(): User[] {
    return this.users.filter(user => user.role === 'admin');
  }
}

const manager = new UserManager();
manager.addUser({ id: 1, name: 'John', email: 'john@example.com', role: 'admin' });
```

### SQL

```sql
-- SQL query examples
CREATE TABLE employees (
    id INT PRIMARY KEY AUTO_INCREMENT,
    first_name VARCHAR(50) NOT NULL,
    last_name VARCHAR(50) NOT NULL,
    email VARCHAR(100) UNIQUE,
    department VARCHAR(50),
    salary DECIMAL(10, 2),
    hire_date DATE
);

INSERT INTO employees (first_name, last_name, email, department, salary, hire_date)
VALUES ('John', 'Doe', 'john.doe@example.com', 'Engineering', 75000.00, '2023-01-15');

SELECT e.first_name, e.last_name, e.department, e.salary
FROM employees e
WHERE e.salary > 50000
ORDER BY e.salary DESC
LIMIT 10;

UPDATE employees
SET salary = salary * 1.1
WHERE department = 'Engineering' AND hire_date < '2023-01-01';
```

### HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Example Page</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Welcome to My Website</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    
    <main>
        <section id="content">
            <p>This is the main content area.</p>
        </section>
    </main>
    
    <footer>
        <p>&copy; 2024 Example Company</p>
    </footer>
</body>
</html>
```

### CSS

```css
/* CSS styling examples */
:root {
    --primary-color: #007bff;
    --secondary-color: #6c757d;
    --font-family: 'Arial', sans-serif;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: var(--font-family);
    line-height: 1.6;
    color: #333;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
}

.btn {
    display: inline-block;
    padding: 10px 20px;
    background-color: var(--primary-color);
    color: white;
    text-decoration: none;
    border-radius: 5px;
    transition: background-color 0.3s ease;
}

.btn:hover {
    background-color: #0056b3;
}

@media (max-width: 768px) {
    .container {
        padding: 10px;
    }
}
```

### JSON

```json
{
  "name": "example-project",
  "version": "1.0.0",
  "description": "An example project configuration",
  "author": {
    "name": "John Doe",
    "email": "john@example.com"
  },
  "dependencies": {
    "express": "^4.18.0",
    "react": "^18.2.0",
    "lodash": "^4.17.21"
  },
  "devDependencies": {
    "jest": "^29.0.0",
    "eslint": "^8.0.0"
  },
  "scripts": {
    "start": "node index.js",
    "test": "jest",
    "lint": "eslint ."
  },
  "keywords": ["example", "demo", "test"]
}
```

### YAML

```yaml
# YAML configuration example
version: '3.8'

services:
  web:
    image: nginx:latest
    ports:
      - "80:80"
      - "443:443"
    volumes:
      - ./html:/usr/share/nginx/html
      - ./config:/etc/nginx/conf.d
    environment:
      - NGINX_HOST=example.com
      - NGINX_PORT=80
    depends_on:
      - api
      - database
  
  api:
    build: ./api
    ports:
      - "3000:3000"
    environment:
      DATABASE_URL: postgresql://user:pass@database:5432/mydb
      NODE_ENV: production
  
  database:
    image: postgres:15
    volumes:
      - db-data:/var/lib/postgresql/data
    environment:
      POSTGRES_USER: user
      POSTGRES_PASSWORD: pass
      POSTGRES_DB: mydb

volumes:
  db-data:
```

### XML

```xml
<?xml version="1.0" encoding="UTF-8"?>
<configuration>
    <appSettings>
        <add key="DatabaseConnection" value="Server=localhost;Database=mydb;" />
        <add key="MaxConnections" value="100" />
        <add key="Timeout" value="30" />
    </appSettings>
    
    <users>
        <user id="1">
            <name>John Doe</name>
            <email>john@example.com</email>
            <role>admin</role>
        </user>
        <user id="2">
            <name>Jane Smith</name>
            <email>jane@example.com</email>
            <role>user</role>
        </user>
    </users>
</configuration>
```

### Bash/Shell

```bash
#!/bin/bash

# Backup script example
BACKUP_DIR="/var/backups"
SOURCE_DIR="/home/user/data"
DATE=$(date +%Y%m%d_%H%M%S)
BACKUP_FILE="backup_${DATE}.tar.gz"

# Create backup directory if it doesn't exist
mkdir -p "$BACKUP_DIR"

# Create backup
echo "Creating backup..."
tar -czf "${BACKUP_DIR}/${BACKUP_FILE}" "$SOURCE_DIR"

# Check if backup was successful
if [ $? -eq 0 ]; then
    echo "Backup created successfully: ${BACKUP_FILE}"
else
    echo "Backup failed!" >&2
    exit 1
fi

# Remove old backups (keep last 7)
find "$BACKUP_DIR" -name "backup_*.tar.gz" -mtime +7 -delete

echo "Backup process completed."
```

### Markdown

```markdown
# Example Markdown

This is a **bold** text and this is *italic*.

## List Example

- Item 1
- Item 2
  - Nested item
  - Another nested item

## Code Example

Inline code: `console.log('Hello')`

> This is a blockquote
```

### Diff

```diff
--- a/file.txt
+++ b/file.txt
@@ -1,5 +1,5 @@
 This is line 1
-This is the old line 2
+This is the new line 2
 This is line 3
-This line will be removed
+This line was added
 This is the last line
```

## Code Blocks Without Language Specification

```
Plain text code block
No syntax highlighting
Just monospace font
```

## Indented Code Blocks

    function indentedCode() {
        return "This is an indented code block";
    }

Another example:

    // Four spaces or one tab
    const x = 42;
    console.log(x);

## Line Numbers in Code

Many markdown renderers support line numbers:

```javascript:line-numbers
function example() {
  const a = 1;
  const b = 2;
  return a + b;
}
```

## Long Code Lines

```javascript
const veryLongFunctionNameThatExceedsTheTypicalLineWidth = (parameterOne, parameterTwo, parameterThree, parameterFour) => {
    return parameterOne + parameterTwo + parameterThree + parameterFour;
};
```

---

**Note**: Syntax highlighting depends on the markdown renderer being used.
