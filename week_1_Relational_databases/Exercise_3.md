



```sql

CREATE TABLE Product(
    maker VARCHAR(255) NOT NULL,
    model VARCHAR(255) NOT NULL,
    type VARCHAR(255) NOT NULL
);

CREATE TABLE PC(
    model VARCHAR(255) NOT NULL,
    speed REAL NOT NULL,
    ram INT NOT NULL,
    hd INT NOT NULL,
    price DECIMAL(10,2) NOT NULL
);

CREATE TABLE Laptop(
    model VARCHAR(255) NOT NULL,
    speed REAL NOT NULL,
    ram INT NOT NULL,
    hd INT NOT NULL,
    screen REAL NOT NULL,
    price DECIMAL(10,2) NOT NULL,
);

CREATE TABLE Printer(
    model VARCHAR(255) NOT NULL,
    color VARCHAR(255) NOT NULL,
    type VARCHAR(255) NOT NULL,
    price DECIMAL(10,2) NOT NULL,
);

ALTER TABLE Printer DROP color;

ALTER TABLE Laptop ADD od VARCHAR(255) DEFAULT 'none'

```