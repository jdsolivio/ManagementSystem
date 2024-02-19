Database for this Project

CREATE TABLE tbl_User
(
    UserID INT IDENTITY(1,1) PRIMARY KEY,
    FullName NVARCHAR(255),
    Username NVARCHAR(50),
    Email NVARCHAR(255),
    Contact NVARCHAR(15),
    Password NVARCHAR(255),
    UserType NVARCHAR(50)
);



CREATE TABLE tbl_TransactionDetails (
    TransactionDetailsID INT IDENTITY(1,1) PRIMARY KEY,
    ProductID INT,
    Tax DECIMAL(10, 2),
    Discount DECIMAL(10, 2),
    Rate DECIMAL(10, 2),
    Quantity INT,
    Total DECIMAL(10, 2)
);


CREATE TABLE tbl_Transaction (
    TransactionID INT IDENTITY(1,1) PRIMARY KEY,
    TransactionType VARCHAR(255),
    SysUser VARCHAR(255),
    GrandTotal DECIMAL(18, 2),
    TransactionDate DATETIME
);


CREATE TABLE tbl_Product
(
    Product_ID INT IDENTITY(1,1) PRIMARY KEY,
    Product_Name NVARCHAR(255),
    Category NVARCHAR(50),
    Rate DECIMAL(10, 2),
    Quantity INT
);




