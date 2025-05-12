<img width="1440" alt="Screenshot 2025-05-12 at 1 15 17 PM" src="https://github.com/user-attachments/assets/99966c30-b9dc-41d8-ac23-46309950bf76" />Micro Project Work

contact email : varalakshmibalasubramani2002@gmail.com

LINK - https://github.com/varalakshmib2002/Micro-Project.git

Title of the Project : Student Enrollment Form 

Description : Student Enrollment Form that will store data in STUDENT-TABLE relation of SCHOOL-DB database.
Input Fields: {Roll-No, Full-Name, Class, Birth-Date, Address, Enrollment-Date}

Primary key: Roll No.

Benefits of using JsonPowerDB : 
Simplest way to retrieve data in a JSON format.
Schema-free, Simple to use, Nimble and In-Memory database.
It is built on top of one of the fastest and real-time data indexing engine - PowerIndeX.
It is low level (raw) form of data and is also human readable.
It helps developers in faster coding, in-turn reduces development cost.
Release History (release of your JsonPowerDB related code on Github)

Additional you can have: 
JsonPowerDB is a Real-time, High Performance, Lightweight and Simple to Use, Rest API based Multi-mode DBMS. JsonPowerDB has ready to use API for Json document DB, RDBMS, Key-value DB, GeoSpatial DB and Time Series DB functionality. JPDB supports and advocates for true serverless and pluggable API development.

Table of contents:
Roll-No
Student Full Name
Class
Birth-Date
Address
Enrollment-Date
SAVE - INSERT
CHANGE - UPDATE
DELETE
RESET

Illustrations
<img width="1440" alt="Screenshot 2025-05-12 at 12 49 37 PM" src="https://github.com/user-attachments/assets/f311513b-ada5-4609-994b-7707d776af04" />

<img width="1426" alt="Screenshot 2025-05-12 at 12 56 50 PM" src="https://github.com/user-attachments/assets/36e3a1e8-70ea-4710-871a-44fef8f964b4" />
<img width="1440" alt="Screenshot 2025-05-12 at 1 13 45 PM" src="https://github.com/user-attachments/assets/af08ecc6-0c86-48ff-a4d2-8ff567d6844d" />
<img width="1440" alt="Screenshot 2025-05-12 at 1 15 17 PM" src="https://github.com/user-attachments/assets/78de7dbf-e18e-427e-9a6b-f652f9e514f4" />
<img width="1440" alt="Screenshot 2025-05-12 at 1 15 00 PM" src="https://github.com/user-attachments/assets/c17ee89c-08be-420d-bf5e-84b7552c4ec6" />
Scope of functionalities : 

Examples of use : can be used foe various other platforms like Online Examination Registration , Job Application , profile creation , and many more other uses .

Project status : Done

Sources :Introduction to JsonPowerDB - V2.0
https://careers.login2explore.com/course/view.php?id=14

Other information Sources :
https://login2explore.com/jpdb/docs.html

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------

STEP BY STEP COURSE DOCUMENTATION :
# JsonPOwerDB
Introduction to JsonPowerDB - V2.0
Login2Xplore 

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Creating a Developer Account and Generating Connection Token : -

Visit: http://api.login2explore.com:5577/user/index.html
REGISTER
After registration check your email-id for password.
Login at http://api.login2explore.com:5577/user/index.html using your email and password received.
First of all change password - Left Navigation >> Change Password.
Login with new password. 

Tools > Token > connection token > Generate (Token needed to communicate with Data Base)

90934669|-31949207107464211|90956059

Token used to execute the API

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Installing Talend API Tester : -

Google > settings > Extensions > Chrome Web store > Talend API Tester - Free Edition > Add to chrome extension


--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Understanding JsonPowerDB and its Features : -

nimble , schema Free , simple to use , in memory and real time , easy to maintain , serverless support , enables multi mode database , power Index , Web services API
Cost efficient , multiple security layers , best performance

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
JsonPowerDB Use case and Benefits : -

any software app that needs backend db
all rdbms use cases
all document db use cases
all key- value db use cases
use cases that needs GeoSpacial/Time series Analytics
Best suited to real - time application for data analytics
Improving existing application reporting/ analytics performance.
Live working HTML, Templates.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
PUT Command - Creating (Inserting) Record : - # IML (JPDB Index Manipulation Language) 
PUT : Insert single record in the database
Token - 90934669|-31949207107464211|90956059

Talend > post
Base url : http://api.login2explore.com:5577
End-point url : /api/iml (mentioned in command when different)

{
    "token": "90934669|-31949207107464211|90956059",
    "cmd": "PUT",
    "dbName": "Employee",
    "rel": "Emp-Rel",
    "jsonStr": {
        "id": "2",
        "name": "Ajay Kailaash",
        "email": "ajaykailaash@gmail.com",
        "mobileno": "9876543210"
    }
}

> Send >

{"data":"{\"rec_no\":[1]}","additionalData":{"processReqType":0,"dbUpdateFlag":true},
"message":"RELATION CREATED, TEMPLATE CREATED FROM JSON, DATA INSERTED, 
Total 1 rows are inserted, Added 0 columns as New Index Columns.","status":200}

Dashboard > Visualize > Jsondb > select Database and Relation

1	12/05/2025, 13:11:58	22 Temple Street, Kanchipuram	05/07/2007	9	12/05/2025	Ajay Kailaash	105

New row - 

{
    "token": "90934669|-31949207107464211|90956059",
    "cmd": "PUT",
    "dbName": "Employee",
    "rel": "Emp-Rel",
    "jsonStr": {
        "id": "2",
        "name": "Ajay Kailaash",
        "email": "ajaykailaash@gmail.com",
        "mobileno": "9876543210"
    }
}
{"data":"{\"rec_no\":[2]}","additionalData":{"processReqType":0,"dbUpdateFlag":true},
"message":"DATA INSERTED, 
Total 1 rows are inserted, Added 0 columns as New Index Columns.","status":200}

Dashboard > Visualize > Jsondb > select Database and Relation

1	12/05/2025, 13:07:24			10	2005-04-20	varalakshmibalasubramani2002@gmail.com			Varalakshmi	9876543210	101	A
2	12/05/2025, 13:09:15	45 Anna Street, Kanchipuram	10/05/2006	10			12/05/2025	Yuvasri			103

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
GET Command - Retrieving Record : - # IRL (JPDB Index Retrieval Language)

Talend - 
Add a project

Name - PUT
Project - JPDB
Service - CRUD
save

GET_BY_KEY : Retrieve single record by json data

Talend > Save as > Name : GET >

POST | http://api.login2explore.com:5577/api/irl

"token": "90932512|-31949274757731994|90949158",

{
   {
    "token": "90934669|-31949207107464211|90956059",
    "dbName": "Employee",
    "cmd": "GET",
    "rel": "Emp-Rel",
    "jsonStr": {
        "name": "Yuvasri"
    }
}
}


{"data"
:"{\"name\":\"aniket\",\"id\":\"2\",\"mobileno\":\"8582887792\",\"email\":\"aniket@gmail.com\"}"
,"message":"DATA RETRIEVED FROM PI","status":200}

Ajax Concepts - A Desktop application feel on web-pages ; -

AJAX - Asynchronous JavaScript And XML.
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
How to use JsonPowerDB in Web Pages

https://drive.google.com/file/d/1e4VN4PAec-Y1iFsj0BN5j0pM7mfed0VQ/view?usp=sharing

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Creating a Web Project in NetBeans : -
![Screenshot (901)](https://user-images.githubusercontent.com/84792843/221233551-732712fd-daef-490f-87fe-107390152150.png)
https://drive.google.com/file/d/1e9u2xj7IY7M2W5v7btigQDT7CofBLdlj/view?usp=sharing

CODE - 

<!DOCTYPE html>
<!--
To change this license header, choose License Headers in Project Properties.
To change this template file, choose Tools | Templates
and open the template in the editor.
-->
<html lang="en">
  <head>
    <title>Bootstrap Example</title>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <link
      rel="stylesheet"
      href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css"
    />
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
  </head>
  <body>
    <div class="container">
      <h2>Vertical (basic) form</h2>
      <form id="empForm" method="post">
        <div class="form-group">
          <span
            ><label for="empId">Employee ID:</label>
            <label id="empIdMsg"> </label
          ></span>

          <input
            type="text"
            class="form-control"
            name="empId"
            id="empId"
            placeholder="Enter Employee ID"
            required
          />
        </div>
        <div class="form-group">
          <label for="empName">Employee Name:</label>
          <input
            type="text"
            class="form-control"
            id="empName"
            placeholder="Enter Employee Name"
            name="empName"
          />
        </div>
        <div class="form-group">
          <label for="empEmail">Email:</label>
          <input
            type="email"
            class="form-control"
            id="empEmail"
            placeholder="Enter Employee Email"
            name="empEmail"
          />
        </div>
        <input
          type="button"
          class="btn btn-primary"
          id="empSave"
          value="Save"
          onclick="saveEmployee();"
        />
      </form>
    </div>

    <script>
      function validateAndGetFormData() {
        var empIdVar = $("#empId").val();
        if (empIdVar === "") {
          alert("Employee ID Required Value");
          $("#empId").focus();
          return "";
        }
        var empNameVar = $("#empName").val();
        if (empNameVar === "") {
          alert("Employee Name is Required Value");
          $("#empName").focus();
          return "";
        }
        var empEmailVar = $("#empEmail").val();
        if (empEmailVar === "") {
          alert("Employee Email is Required Value");
          $("#empEmail").focus();
          return "";
        }
        var jsonStrObj = {
          empId: empIdVar,
          empName: empNameVar,
          empEmail: empEmailVar,
        };
        return JSON.stringify(jsonStrObj);
      }

      // This method is used to create PUT Json request.
      function createPUTRequest(connToken, jsonObj, dbName, relName) {
        var putRequest =
          "{\n" +
          '"token" : "' +
          connToken +
          '",' +
          '"dbName": "' +
          dbName +
          '",\n' +
          '"cmd" : "PUT",\n' +
          '"rel" : "' +
          relName +
          '",' +
          '"jsonStr": \n' +
          jsonObj +
          "\n" +
          "}";
        return putRequest;
      }

      function saveEmployee() {
        // validate form data

        // create JPDB request string - token , dbname , relation name ...

        // Execute this request

        //Reset the form data

        var jsonStr = validateAndGetFormData();
        if (jsonStr === "") {
          return;
        }
        var putReqStr = createPUTRequest(
          "90936861|-31948784479254024|90932362",

          jsonStr,
          "SAMPLE",
          "EMP-REL"
        );

        alert(putReqStr);
        jQuery.ajaxSetup({ async: false });
        /* 
          var resultObj = executeCommand(
          putReqStr,
          "http://api.login2explore.com:5577",
          "/api/iml"
        );

        */

        jQuery.ajaxSetup({ async: true });
        alert(JSON.stringify(resultObj));
        resetForm();
      }
    </script>
  </body>
</html>


--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Saving data in JPDB from HTML form :-
![image](https://user-images.githubusercontent.com/84792843/221236356-22fa3e5d-9e1d-4b6e-bead-e28ee931f113.png)

CODE --

<!DOCTYPE html>
<!--
To change this license header, choose License Headers in Project Properties.
To change this template file, choose Tools | Templates
and open the template in the editor.
-->
<html lang="en">
  <head>
    <title>Bootstrap Example</title>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <link
      rel="stylesheet"
      href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css"
    />
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
  </head>
  <body>
    <div class="container">
      <h2>Vertical (basic) form</h2>
      <form id="empForm" method="post">
        <div class="form-group">
          <span
            ><label for="empId">Employee ID:</label>
            <label id="empIdMsg"> </label
          ></span>

          <input
            type="text"
            class="form-control"
            name="empId"
            id="empId"
            placeholder="Enter Employee ID"
            required
          />
        </div>
        <div class="form-group">
          <label for="empName">Employee Name:</label>
          <input
            type="text"
            class="form-control"
            id="empName"
            placeholder="Enter Employee Name"
            name="empName"
          />
        </div>
        <div class="form-group">
          <label for="empEmail">Email:</label>
          <input
            type="email"
            class="form-control"
            id="empEmail"
            placeholder="Enter Employee Email"
            name="empEmail"
          />
        </div>
        <input
          type="button"
          class="btn btn-primary"
          id="empSave"
          value="Save"
          onclick="saveEmployee();"
        />
      </form>
    </div>

    <script>
      function validateAndGetFormData() {
        var empIdVar = $("#empId").val();
        if (empIdVar === "") {
          alert("Employee ID Required Value");
          $("#empId").focus();
          return "";
        }
        var empNameVar = $("#empName").val();
        if (empNameVar === "") {
          alert("Employee Name is Required Value");
          $("#empName").focus();
          return "";
        }
        var empEmailVar = $("#empEmail").val();
        if (empEmailVar === "") {
          alert("Employee Email is Required Value");
          $("#empEmail").focus();
          return "";
        }
        var jsonStrObj = {
          empId: empIdVar,
          empName: empNameVar,
          empEmail: empEmailVar,
        };
        return JSON.stringify(jsonStrObj);
      }

      // This method is used to create PUT Json request.
      function createPUTRequest(connToken, jsonObj, dbName, relName) {
        var putRequest =
          "{\n" +
          '"token" : "' +
          connToken +
          '",' +
          '"dbName": "' +
          dbName +
          '",\n' +
          '"cmd" : "PUT",\n' +
          '"rel" : "' +
          relName +
          '",' +
          '"jsonStr": \n' +
          jsonObj +
          "\n" +
          "}";
        return putRequest;
      }

      function executeCommand(reqString, dbBaseUrl, apiEndPointUrl) {
        var url = dbBaseUrl + apiEndPointUrl;
        var jsonObj;
        $.post(url, reqString, function (result) {
          jsonObj = JSON.parse(result);
        }).fail(function (result) {
          var dataJsonObj = result.responseText;
          jsonObj = JSON.parse(dataJsonObj);
        });
        return jsonObj;
      }

      function resetForm() {
        $("#empId").val("");
        $("#empName").val("");
        $("#empEmail").val("");
        $("#empId").focus();
      }

      function saveEmployee() {
        // validate form data

        // create JPDB request string - token , dbname , relation name ...

        // Execute this request

        //Reset the form data

        var jsonStr = validateAndGetFormData();
        if (jsonStr === "") {
          return;
        }
        var putReqStr = createPUTRequest(
          "90932512|-31949274757731994|90949158",
          jsonStr,
          "SAMPLE",
          "EMP-REL"
        );

        alert(putReqStr);

        jQuery.ajaxSetup({ async: false });
        var resultObj = executeCommand(
          putReqStr,
          "http://api.login2explore.com:5577",
          "/api/iml"
        );
        jQuery.ajaxSetup({ async: true });

        alert(JSON.stringify(resultObj));
        resetForm();
      }
    </script>
  </body>
</html>


--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
JPDB using jpdb common js - A Javascript library to make it even easy and fast for developers :-

Code - 

<!DOCTYPE html>
<!--
To change this license header, choose License Headers in Project Properties.
To change this template file, choose Tools | Templates
and open the template in the editor.
-->
<html lang="en">
  <head>
    <title>Bootstrap Example</title>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <link
      rel="stylesheet"
      href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css"
    />
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
    <script src="https://login2explore.com/jpdb/resources/js/0.0.3/jpdb-commons.js"></script>
  </head>
  <body>
    <div class="container">
      <h2>Vertical (basic) form</h2>
      <form id="empForm" method="post">
        <div class="form-group">
          <span
            ><label for="empId">Employee ID:</label>
            <label id="empIdMsg"> </label
          ></span>

          <input
            type="text"
            class="form-control"
            name="empId"
            id="empId"
            placeholder="Enter Employee ID"
            required
          />
        </div>
        <div class="form-group">
          <label for="empName">Employee Name:</label>
          <input
            type="text"
            class="form-control"
            id="empName"
            placeholder="Enter Employee Name"
            name="empName"
          />
        </div>
        <div class="form-group">
          <label for="empEmail">Email:</label>
          <input
            type="email"
            class="form-control"
            id="empEmail"
            placeholder="Enter Employee Email"
            name="empEmail"
          />
        </div>
        <input
          type="button"
          class="btn btn-primary"
          id="empSave"
          value="Save"
          onclick="saveEmployee();"
        />
      </form>
    </div>

    <script>
      function validateAndGetFormData() {
        var empIdVar = $("#empId").val();
        if (empIdVar === "") {
          alert("Employee ID Required Value");
          $("#empId").focus();
          return "";
        }
        var empNameVar = $("#empName").val();
        if (empNameVar === "") {
          alert("Employee Name is Required Value");
          $("#empName").focus();
          return "";
        }
        var empEmailVar = $("#empEmail").val();
        if (empEmailVar === "") {
          alert("Employee Email is Required Value");
          $("#empEmail").focus();
          return "";
        }
        var jsonStrObj = {
          empId: empIdVar,
          empName: empNameVar,
          empEmail: empEmailVar,
        };
        return JSON.stringify(jsonStrObj);
      }

      function resetForm() {
        $("#empId").val("");
        $("#empName").val("");
        $("#empEmail").val("");
        $("#empId").focus();
      }

      function saveEmployee() {
        // validate form data

        // create JPDB request string - token , dbname , relation name ...

        // Execute this request

        //Reset the form data

        var jsonStr = validateAndGetFormData();
        if (jsonStr === "") {
          return;
        }
        var putReqStr = createPUTRequest(
          "90932512|-31949274757731994|90949158",
          jsonStr,
          "SAMPLE",
          "EMP-REL"
        );

        alert(putReqStr);

        jQuery.ajaxSetup({ async: false });
        var resultObj = executeCommandAtGivenBaseUrl(
          putReqStr,
          "http://api.login2explore.com:5577",
          "/api/iml"
        );
        jQuery.ajaxSetup({ async: true });

        alert(JSON.stringify(resultObj));
        resetForm();
      }
    </script>
  </body>
</html>


2	2/24/2023, 10:38:48 PM	payel@gmail.com	61	payel jain

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Test - Serverless JPDB
Test your knowledge 

Attempts allowed: 5

Time limit: 5 mins

Grading method: Highest grade

Summary of your previous attempts
Attempt	State	Grade / 5.00	Review	Feedback
1	Finished
Submitted Friday, 24 February 2023, 10:45 PM
5.00		
Congratulations!! Excellent Performance! Keep it Up.

Highest grade: 5.00 / 5.00.
Overall feedback
Congratulations!! Excellent Performance! Keep it Up.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Useful Commands to Practice
JPDB Documentation Page: http://login2explore.com/jpdb/docs.html#jpdb-command-request 

Practice following commands on the above JsonPowerDB documentation link:

1. IML Commands

PUT
PUT_ALL
UPDATE
REMOVE
2. IRL Commands

GET_BY_KEY
GET_BY_RECORD

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Development of Employee Form with Control Buttons

CODE :-
<!DOCTYPE html>
<!--
To change this license header, choose License Headers in Project Properties.
To change this template file, choose Tools | Templates
and open the template in the editor.
-->
<html lang="en">
  <head>
    <title>Employee Form using JPDB</title>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <link
      rel="stylesheet"
      href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css"
    />
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
    <script src="https://login2explore.com/jpdb/resources/js/0.0.3/jpdb-commons.js"></script>
  </head>
  <body>
    <div class="container">
      <h2>Employee Form Using the JPDB API</h2>
      <form id="empForm" method="post">
        <div class="form-group">
          <span
            ><label for="empId">Employee ID:</label>
            <label id="empIdMsg"> </label
          ></span>

          <input
            type="text"
            class="form-control"
            onchange="getEmp()"
            name="empId"
            id="empId"
            placeholder="Enter Employee ID"
            required
          />
        </div>
        <div class="form-group">
          <label for="empName">Employee Name:</label>
          <input
            type="text"
            class="form-control"
            id="empName"
            placeholder="Enter Employee Name"
            name="empName"
          />
        </div>
        <div class="form-group">
          <label for="empEmail">Email:</label>
          <input
            type="email"
            class="form-control"
            id="empEmail"
            placeholder="Enter Employee Email"
            name="empEmail"
          />
        </div>
        <input
          type="button"
          class="btn btn-primary"
          id="empSave"
          value="Save"
          onclick="saveEmployee();"
        />
        <input
          type="button"
          class="btn btn-primary"
          id="empChange"
          value="Change"
          onclick="changeEmployee();"
        />
        <input
          type="button"
          class="btn btn-primary"
          id="empReset"
          value="Reset"
          onClick="window.location.reload()"
        />
      </form>
    </div>

    <script>
      function validateAndGetFormData() {
        var empIdVar = $("#empId").val();
        if (empIdVar === "") {
          alert("Employee ID Required Value");
          $("#empId").focus();
          return "";
        }
        var empNameVar = $("#empName").val();
        if (empNameVar === "") {
          alert("Employee Name is Required Value");
          $("#empName").focus();
          return "";
        }
        var empEmailVar = $("#empEmail").val();
        if (empEmailVar === "") {
          alert("Employee Email is Required Value");
          $("#empEmail").focus();
          return "";
        }
        var jsonStrObj = {
          empId: empIdVar,
          empName: empNameVar,
          empEmail: empEmailVar,
        };
        return JSON.stringify(jsonStrObj);
      }

      function resetForm() {
        $("#empId").val("");
        $("#empName").val("");
        $("#empEmail").val("");
        $("#empId").focus();
      }

      function saveEmployee() {
        // validate form data

        // create JPDB request string - token , dbname , relation name ...

        // Execute this request

        //Reset the form data

        var jsonStr = validateAndGetFormData();
        if (jsonStr === "") {
          return;
        }
        var putReqStr = createPUTRequest(
          "90932512|-31949274757731994|90949158",
          jsonStr,
          "SAMPLE",
          "EMP-REL"
        );

        alert(putReqStr);

        jQuery.ajaxSetup({ async: false });
        var resultObj = executeCommandAtGivenBaseUrl(
          putReqStr,
          "http://api.login2explore.com:5577",
          "/api/iml"
        );
        jQuery.ajaxSetup({ async: true });

        alert(JSON.stringify(resultObj));
        resetForm();
      }
    </script>
  </body>
</html>

![image](https://user-images.githubusercontent.com/84792843/221276871-9de54244-d0c2-4e88-aca5-d6802567fa5e.png)


--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Micro Project Work

Student Enrollment Form

CODE - 

<!DOCTYPE html>
<!--
To change this license header, choose License Headers in Project Properties.
To change this template file, choose Tools | Templates
and open the template in the editor.
-->
<html lang="en">
  <head>
    <title>Micro Project Work</title>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <link
      rel="stylesheet"
      href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css"
    />
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
    <script src="https://login2explore.com/jpdb/resources/js/0.0.3/jpdb-commons.js"></script>
  </head>
  <body>
    <div class="container">
      <h2>Student Enrollment Form (Micro Project Work)</h2>
      <form id="stuForm" method="post">
        <div class="form-group">
          <span
            ><label for="stuId">Roll-No:</label> <label id="stuIdMsg"> </label
          ></span>

          <input
            type="text"
            class="form-control"
            onchange="getStu()"
            name="stuId"
            id="stuId"
            placeholder="Enter Roll-No"
            required
          />
        </div>

        <div class="form-group">
          <label for="stuName">Student Full Name:</label>
          <input
            type="text"
            class="form-control"
            id="stuName"
            placeholder="Enter Full Name"
            name="stuName"
          />
        </div>

        <div class="form-group">
          <label for="stuClass">Class:</label>
          <input
            type="text"
            class="form-control"
            id="stuClass"
            placeholder="Enter Class"
            name="stuClass"
          />
        </div>

        <div class="form-group">
          <label for="stuDOB">Birth-Date:</label>
          <input
            type="date"
            class="form-control"
            id="stuDOB"
            placeholder="Enter Birth-Date"
            name="stuDOB"
          />
        </div>

        <div class="form-group">
          <label for="stuAddress">Address:</label>
          <input
            type="text"
            class="form-control"
            id="stuAddress"
            placeholder="Enter Address"
            name="stuAddress"
          />
        </div>

        <div class="form-group">
          <label for="stuEnrollDate">Enrollment-Date:</label>
          <input
            type="date"
            class="form-control"
            id="stuEnrollDate"
            placeholder="Enter Enrollment-Date"
            name="stuEnrollDate"
          />
        </div>

        <input
          type="button"
          class="btn btn-primary"
          id="empSave"
          value="Save"
          onclick="saveData();"
        />
        <input
          type="button"
          class="btn btn-primary"
          id="empChange"
          value="Change"
          onclick="changeData();"
        />
        <input
          type="button"
          class="btn btn-primary"
          id="empReset"
          value="Reset"
          onClick="resetForm()"
        />
        <!-- window.location.reload() -->
      </form>
    </div>

    <script>
      function validateAndGetFormData() {
        var stuIdVar = $("#stuId").val();
        if (stuIdVar === "") {
          alert("Student Roll-No Required Value");
          $("#stuId").focus();
          return "";
        }
        var stuNameVar = $("#stuName").val();
        if (stuNameVar === "") {
          alert("Student Name is Required Value");
          $("#stuName").focus();
          return "";
        }
        var stuClassVar = $("#stuClass").val();
        if (stuClassVar === "") {
          alert("Student Class is Required Value");
          $("#stuClass").focus();
          return "";
        }

        var stuDOBVar = $("#stuDOB").val();
        if (stuDOBVar === "") {
          alert("Student Birth-Date is Required Value");
          $("stuDOB").focus();
          return "";
        }

        var stuAddressVar = $("#stuAddress").val();
        if (stuAddressVar === "") {
          alert("Student Address is Required Value");
          $("#stuAddress").focus();
          return "";
        }

        var stuEnrollDateVar = $("stuEnrollDate").val();
        if (stuEnrollDateVar === "") {
          alert("Student Enrollment-Date is Required Value");
          $("stuEnrollDate").focus();
          return "";
        }

        var jsonStrObj = {
          stuId: stuIdVar,
          stuName: stuNameVar,
          stuClass: stuClassVar,
          stuDOB: stuDOBVar,
          stuAddress: stuAddressVar,
          stuEnrollDate: stuEnrollDateVar,
        };
        return JSON.stringify(jsonStrObj);
      }

      function getstuIdASJsonObj() {
        var stuid = $("#stuid").val();
        var jsonStr = {
          id: stuid,
        };
        return JSON.stringify(jsonStr);
      }

      function getStu() {
        var stuIdJsonObj = getstuIdASJsonObj();
        var getRequest = createGET_BY_KEYRequest(
          connToken,
          stuDBName,
          stuRelationName,
          stuIdJsonObj
        );
        jQuery.ajaxSetup({ async: false });
        var resJsonObj = executeCommandAtGivenBaseUrl(
          getRequest,
          jpdbBaseURL,
          jpdbURL
        );
        jQuery.ajaxSetup({ async: true });
        if (resJsonObj.status === 400) {
          $("#save").prop("disabled", flase);
          $("#reset").prop("disabled", false);
          $("#stuname").focus();
        } else if (resJsonObj.status === 200) {
          $("#stuid").prop("disabled", true);
          fillData(resJsonObj);
          $("#change").prop("disabled", false);
          $("#reset").prop("disabled", false);
          $("#stuname").focus();
        }
      }

      function resetForm() {
        $("#stuId").val("");
        $("#stuName").val("");
        $("#stuClass").val("");
        $("#stuDOB").val("");
        $("#stuAddress").val("");
        $("#stuEnrollDate").val("");
        $("#stuId").focus();
      }

      function changeData() {
        $("#change").prop("disabled", true);
        jsonChg = validateData();
        var updateRequest = createUPDATERecordRequest(
          ConnToken,
          jsonChg,
          stuDBName,
          stuRelationName,
          localStorage.getItem("recno")
        );
        jQuery.ajaxSetup({ async: falses });
        var resJsonObj = executeCommandAtGivenBaseUrl(
          updateRequest.jpdBaseURL,
          jpdbIML
        );
        jQuery.ajaxSetup({ async: true });
        console.log(resJsonObj);
        resetForm();
        $("#stuID").focus();
      }

      function saveData() {
        // validate form data

        // create JPDB request string - token , dbname , relation name ...

        // Execute this request

        //Reset the form data

        var jsonStr = validateAndGetFormData();
        if (jsonStr === "") {
          return;
        }
        var putReqStr = createPUTRequest(
          "90932512|-31949274757731994|90949158",
          jsonStr,
          "SCHOOL-DB",
          "STUDENT-TABLE"
        );

        alert(putReqStr);

        jQuery.ajaxSetup({ async: false });
        var resultObj = executeCommandAtGivenBaseUrl(
          putReqStr,
          "http://api.login2explore.com:5577",
          "/api/iml"
        );
        jQuery.ajaxSetup({ async: true });

        alert(JSON.stringify(resultObj));
        resetForm();
      }
    </script>
  </body>
</html>
![image](https://user-images.githubusercontent.com/84792843/221289611-acb5c361-c3f7-4221-957e-5a7f9c489426.png)

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Published Micro Project Code to Github
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
More Commands to Practice
JPDB Documentation Page: http://login2explore.com/jpdb/docs.html#jpdb-command-request

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Test - Interactive JPDB
Test your knowledge 

Attempts allowed: 5

Time limit: 5 mins

Grading method: Highest grade

Highest grade: 3.00 / 4.00.
Overall feedback
Congratulations!! Excellent Performance! Keep it Up.

