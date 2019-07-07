JDBC Project:
1) Java netbeans(8.2 ide) code :
i) The code is in two classes – RegisterFrame.java and
DisplayFrame.java, under the project name ‘CaseStudy’
inside the package ‘casestudy’.
ii) The first class contains the frame for entering the
candidate details, while the second frame, which opens
simultaneously, displays the details of the last five
candidates who have registered.
iii) As soon as the candidate enters its details, it gets
reflected in the second frame(DisplayFrame).

2) MySql database :
i) First added the connector : mysql-connector-java-
8.0.15.jar In the library of the java project (JAR file).

Then connected the RegisterFrame class with the mysql
database using
url –jdbc:mysql://localhost:3306/customerdetails
username-root
password-root123

ii) Created the Database ‘customerdetails’, with the table
name ‘customer’

CREATE TABLE `customer` (
`UniqueToken` int(11) NOT NULL AUTO_INCREMENT,
`FirstName` varchar(255) NOT NULL,
`LastName` varchar(255) DEFAULT NULL,
`Age` int(11) DEFAULT NULL,
`Phone` varchar’(20) DEFAULT NULL,
PRIMARY KEY (`UniqueToken`)
) ENGINE=InnoDB AUTO_INCREMENT=2 DEFAULT
CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci