# ASP.NET Core Minimal API for complete beginners course - Code examples

This repository contains the source code examples for the videos featured in the [ASP.NET Core Minimal API for complete beginners course](https://www.roundthecode.com/min1).

## Code examples
Each video that includes a code example has two corresponding branches:
- `-begin`: The code state at the beginning of the video
- `-end`: The code state at the end of the video

You can watch [the video](https://www.udemy.com/course/6838899/learn/lecture/53513933) to determine which branch you need to download for the lesson you're following.

## Download the database
If you're following the course from the beginning, you'll learn how to create the database using Entity Framework Core migrations.

However, if you want to skip ahead or encounter issues creating the database, you can [download a database backup](https://github.com/RoundTheCode/Minimal-APIs-for-complete-beginners/blob/s03/l02-end/ToDo%20database%20backup.bacpac) instead.

The backup is provided as a `.bacpac` file. To import it, you'll need [SQL Server Management Studio (SSMS)](https://learn.microsoft.com/en-us/ssms/).

### Importing the database
- Open SSMS and connect to the SQL Server instance where you want to import the database.
- Right-click **Databases** and select **Import Data-tier Application...***.
- Click **Next**, then under **Import from local disk**, select **Browse...** and locate the `.bacpac` file.
- Follow the remaining steps and click **Finish** to complete the import.

Finally, ensure your connection string is configured correctly in `Api/appsettings.Development.json`. Verify that the server and database name match your SQL Server setup.