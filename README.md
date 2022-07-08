<a href="https://fontmeme.com/ben-10-font/"><img src="https://fontmeme.com/permalink/220615/a104da11aabf99c44433306f7cd6e9d8.png" alt="ben-10-font" border="0"></a>


![At'choo Banner](AtchooClient/wwwroot/img/banner-small.png)

#### By Meron Tekie, Mark McConnel, Caleb Coughenour, Marcus Lorenzo, Jake Edgar, and Evgeniya Meshuris

### A web application for an allergy-themed dating app 


![ezgif com-gif-maker (3)](https://user-images.githubusercontent.com/100096239/177896274-19741eb6-9c19-4eed-9f5c-e57fc4ad1a5e.gif)



### 🖥️ Technologies Used 

<br><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg" width="60" height="60"/> 
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/dot-net/dot-net-plain-wordmark.svg" width="60" height="60"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-plain-wordmark.svg" width="60" height="60"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-plain-wordmark.svg" width="60" height="60"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-plain.svg" width="60" height="60"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-plain-wordmark.svg" width="60" height="60"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-plain-wordmark.svg" width="60" height="60"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original-wordmark.svg" width="60" height="60"/><br>

## ✅ Description

A web application that allows a user to create authentication and login to the website with their authenticated credentials. After becoming an authorized user, a user can create a user profile and add their allergies. Once their user profile and allergies have been added our application will match users with other users with complimentary/similar allergies for dating purposes. The application has full crud functionality for authenticated users. Non-authenticated users can interact with the site and see the full list of allergies.

## ⚙️ Setup/Installation Requirements

* First, make sure you have MySql Workbench downloaded and properly installed. You will also need a text editor and a command-line that you are comfortable with. 

* In your command line navigate to your desktop directory and clone this project <https://github.com/CalebCoughenour/AtchooClient.Solution>

* Open the project in your preferred text editor, we recommend VSCode.
* In the root directory, confirm there is a .gitignore file
* Add:

    ```
    */obj/
    */bin/
    *.vscode
    */appsettings.json
    ```

* To the .gitignore file. It will keep your repository clean of unnecessary files and protect your database from unauthorized access
* Create an appsetting.json file at the root directory
* Open the appsetting.json file and enter: 

* To create the database please do as follows:

  * First create a file using the *touch* command in your command line, at the root of the project directory called "appsettings.json" and in that file add the following code, but substituting the text in the brackets for your own information. 

  ```
      { 
        "ConnectionStrings": { 
          "DefaultConnection": "Server=localhost;Port=3306;database=[your_database];uid=[Your ID];pwd=[Your Password];" 
        }
      }
  ```
* Run the following from the project directory of ```AtchooClient```
  * Run ```dotnet add package Microsoft.EntityFrameworkCore -v 5.0.0```
  * Run ```dotnet add package Pomelo.EntityFrameworkCore.MySql -v 5.0.0-alpha.2```
  * Run ```dotnet add package Microsoft.EntityFrameworkCore.Proxies -v 5.0.0```
  * Run ```dotnet add package Microsoft.AspNetCore.Identity.EntityFrameworkCore -v 5.0.0```
* Once all of the necessary set-up is in place, In your command line navigate to the directory "AtchooClient" and run the following commands in order:
    * ```dotnet restore```
    * ```dotnet build```
    * ```dotnet ef migrations add Initial```
* Once we have verified that the migration looks correct and made any necessary changes, we'll run the following commands: 
    * ```dotnet ef database update```
    * ```dotnet run```

* To interact with the local host website navigate to the project directory and run ```dotnet run```
* Click on  <http://localhost:5000> and you are in there like swimwear!

## Known 🐛 Bugs

* If no profile image is uploaded to a user profile it shows a broken image link
* Users can enter the direct URL to other profiles and Edit/Delete that respective profile
* Users can see other profiles listed for an allergy even if they don't have that allergy listed in their profile 

## 🎫 License 👈

Licensed under the [MIT License](LICENSE).
Copyright (c) 2022 <br>Meron Tekie [![Linkedin Badge](https://img.shields.io/badge/LinkedIn-blue?style=flat&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/meron-tekie/) ----- Mark McConnel [![Linkedin Badge](https://img.shields.io/badge/LinkedIn-blue?style=flat&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/mark-mcconnell1/) ----- Caleb Coughenour [![Linkedin Badge](https://img.shields.io/badge/LinkedIn-blue?style=flat&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/caleb-coughenour/) <br>Marcus Lorenzo [![Linkedin Badge](https://img.shields.io/badge/LinkedIn-blue?style=flat&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/marcusanthonylorenzo/) ----- Jake Edgar [![Linkedin Badge](https://img.shields.io/badge/LinkedIn-blue?style=flat&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/jake-m-edgar/) ----- Evgeniya Meshuris [![Linkedin Badge](https://img.shields.io/badge/LinkedIn-blue?style=flat&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/evmeshuris/)
