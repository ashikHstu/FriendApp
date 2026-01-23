# Environment Preparation for FriendApp

## 1. Prerequisites
* **.NET SDK**: Download and install from [dotnet.microsoft.com](https://dotnet.microsoft.com/en-us/download)
  * Check version: `dotnet --version`
* **Node.js & npm**: Download and install from [nodejs.org](https://nodejs.org/en/download)
  * Check version: `node -v` and `npm -v`

---

## 2. Project Setup
To ignore permission issues, create a folder under your **User** folder in the `C:` drive. Execute the following commands inside that folder:

```bash
# Create the solution file
dotnet new sln

# Create a Web API project named "API" with controllers
dotnet new webapi -controllers -n API

# Add the API project to the solution list
dotnet sln add API

# Verify the list of projects
dotnet sln list

# Open the project in VS Code
code .

# Run the dotnet project (go inside the API project first, cd API)
cd API
dotnet run
```

## 3. Visual Studio Code Extensions
Install the following extensions to set up your environment:

* **.Net Install tool**
* **C#**
* **C# Dev Kit**
* **Material Icon Theme** (Just to improve the look)
* **NuGet Gallery**

## 4. dotnet certificate import
* **dotnet dev-certs https -h**   (to see list of valid operations)
* **dotnet dev-certs https --check**
* **dotnet dev-certs https --clean** (to remove the certificate)
* **dotnet dev-certs https --trust**