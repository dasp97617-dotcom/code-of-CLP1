CREATE DATABASE CLP

CREATE TABLE COUNTRY(
    countryID INT,
    countryID INT NOT NULL,
    country_name VARCHAR(50),
    continent VARCHAR(50),
    currency VARCHAR(50)
);
CREATE TABLE Department(
    DepartmentID INT NOT NULL,
    DepartmentID INT,
    DeptName VARCHAR(50),
    countryID INT
);
CREATE TABLE Employee(
    EmpID INT NOT NULL,
    EmpID INT,
    Empname VARCHAR(50),
    Deptid INT
);
CREATE TABLE Folder(
    FolderID INT NOT NULL,
    FolderID INT,
    EmpID INT,
    AccessType VARCHAR(50)
);
INSERT INTO COUNTRY
VALUES(170,"Bangladesh","South Asia","TAKA");
INSERT INTO COUNTRY
VALUES(171, "India", "South Asia", "Rupi");
INSERT INTO COUNTRY
VALUES(172, "USA", "America", "Dollar");
INSERT INTO COUNTRY
VALUES(173, "Spain", "Europe", "Euro");
INSERT INTO COUNTRY
VALUES(174, "Kuwet", "north", "Dinar");

INSERT INTO Department
VALUES(1701, "CSE", 170);
INSERT INTO Department
VALUES(1701, "Law", 171);
INSERT INTO Department
VALUES(1702, "GBS", 172);
INSERT INTO Department
VALUES(1703, "BBA", 173);
INSERT INTO Department
VALUES(1704, "SWE", 174);

INSERT INTO Employee
VALUES(1700, "Rahim", 1701);
INSERT INTO Employee
VALUES(1711, "Karim", 1701);
INSERT INTO Employee
VALUES(1722, "Borak", 1702);
INSERT INTO Employee
VALUES(1733, "Messi", 1703);
INSERT INTO Employee
VALUES(1744, "Tarek", 1704);

INSERT INTO Folder
VALUES(1000, 1700, "Private");
INSERT INTO Folder
VALUES(2000, 1711, "Default");
INSERT INTO Folder
VALUES(3000, 1722, "Public");
INSERT INTO Folder
VALUES(4000, 1733, "Private");
INSERT INTO Folder
VALUES(5000, 1744, "Public");

SELECT * (ALL TABLES)
