# Philips C# Training - July 2019

This repository contains the source code and examples for the Philips C# Training conducted in July 2019.

## Code Wiki

This wiki provides an overview of the different projects and examples included in this training repository.

### 1. C# Demos (`CSharpDemos`)

This project contains a collection of console applications demonstrating various fundamental concepts in C#.

**Location:** `CSharpDemos/SampleConApp`

**Topics Covered:**

*   Abstract Classes (`AbstractClasses.cs`)
*   Arrays (`ArraysExample.cs`)
*   Attributes (`AttributesExample.cs`)
*   Custom Collections (`CustomCollectionDemo.cs`, `EmployeeCollectionDemo.cs`)
*   Data Types (`DataTypes.cs`)
*   Delegates (`DelegatesExample.cs`, `DelegatesInUsage.cs`)
*   Using DLLs (`DllClient.cs`)
*   Generics (`GenericsDemo.cs`)
*   Inheritance and OOP (`InheritanceDemo.cs`, `OOPConcepts.cs`, `MethodOverriding.cs`)
*   Interfaces (`Interfaces.cs`)
*   Reflection (`ReflectionExample.cs`)
*   Structures (`Structures.cs`)

### 2. Reflection Recap (`ReflectionRecap`)

This project is a practical example of using C# Reflection.

**Location:** `ReflectionRecap/ReflectionClient`

**Functionality:**

The program dynamically loads a .NET assembly (DLL) specified in the `App.config` file. It then inspects the types and methods within the assembly, and allows the user to select a method to invoke at runtime. The program prompts for parameter values if the selected method has any.

### 3. Windows Communication Foundation (WCF) Examples (`WCF/WCFExamples`)

This solution demonstrates various aspects of WCF.

**Projects:**

*   **`SampleWcfLib`**: A WCF Service Library project that defines the service contract (`IService`) and implements the service (`Service`).
*   **`SelfHostinApp`**: A console application that hosts the WCF service. This allows the service to run without needing IIS.
*   **`WcfWinService`**: A Windows Service project for hosting the WCF service.
*   **`WcfClient`**: A console application that acts as a client, consuming the methods exposed by the WCF service.

### 4. ASP.NET Web API (`WebAPI`)

This project demonstrates how to create a simple RESTful API using ASP.NET Core Web API.

**Location:** `WebAPI/EmployeeService`

**API Endpoints:**

The `EmployeeController.cs` defines the following endpoints for managing employee data:

*   `GET /api/Employee`: Retrieves a list of all employees.
*   `GET /api/Employee/{id}`: Retrieves a single employee by their ID.
*   `POST /api/Employee`: Adds a new employee to the database.
*   `PUT /api/Employee`: Updates an existing employee's information.

The API uses a data access library (`ClassLibrary1`) to interact with a data source.
