# 🌊 Drizzle - Easy PostgreSQL CRUD for Everyone

## 🔗 Download Drizzle Now
[![Download Drizzle](https://img.shields.io/badge/Download%20Drizzle-Click%20Here-brightgreen)](https://github.com/amanueln641/Drizzle/releases)

## 🚀 Getting Started
Drizzle is designed for users who want a simple way to manage their PostgreSQL databases. With Drizzle, you can create, read, update, and delete (CRUD) data effortlessly. You don’t need a technical background to use it. Follow the steps below to get started.

## 💻 System Requirements
Before installing Drizzle, make sure your computer meets the following requirements:
- **Operating System:** Windows, macOS, or Linux
- **Node.js:** Version 12 or later installed
- **PostgreSQL:** A running PostgreSQL database instance

## 📥 Download & Install
To get Drizzle, visit the Releases page and find the latest version:

[Visit the Releases Page to Download](https://github.com/amanueln641/Drizzle/releases)

1. Click on the link above.
2. On the Releases page, look for the latest release version.
3. Download the appropriate file for your operating system.

For example:
- **Windows:** Look for a file named `drizzle-windows.zip`
- **macOS:** Choose `drizzle-macos.zip`
- **Linux:** Select `drizzle-linux.tar.gz`

Once downloaded, follow these steps to install:

### Windows Installation
1. Unzip the downloaded file.
2. Open the folder and double-click `drizzle.exe` to start.
3. Follow the setup instructions.

### macOS Installation
1. Unzip the downloaded file.
2. Open Terminal and navigate to the folder.
3. Run the command `./drizzle`.

### Linux Installation
1. Extract the tar.gz file using the command:
   ```
   tar -xzf drizzle-linux.tar.gz
   ```
2. Navigate into the extracted directory.
3. Run the command `./drizzle`.

## 📊 Features
- **TypeScript Built:** Drizzle uses TypeScript to ensure your data is handled safely and effectively.
- **Easy Migrations:** Keep your database in sync with easy-to-use migration tools.
- **Typesafe:** You get strong typing, reducing errors when working with data.

## 🔧 Configuration
After you install Drizzle, configure it to connect to your PostgreSQL database:

1. Open the `config.json` file located in the Drizzle folder.
2. Modify the settings to match your database connection:
   ```json
   {
     "host": "localhost",
     "port": 5432,
     "user": "your_username",
     "password": "your_password",
     "database": "your_database"
   }
   ```
3. Save the file.

## 📚 Using Drizzle
### Create Data
To create new data, you can use simple commands. For example, to add a user:
```javascript
await drizzle.create('users', { name: 'John Doe' });
```

### Read Data
To retrieve data, use the following command:
```javascript
const users = await drizzle.read('users');
console.log(users);
```

### Update Data
To update data, use:
```javascript
await drizzle.update('users', { id: 1, name: 'Jane Doe' });
```

### Delete Data
To delete a record, run:
```javascript
await drizzle.delete('users', { id: 1 });
```

## 🌐 Community Support
If you have questions or need help, visit our [Discussion Page](https://github.com/amanueln641/Drizzle/discussions). You can ask questions, get tips, and share your experiences with other users.

## 📄 License
Drizzle is licensed under the MIT License. You are free to use and modify the software as you wish.

## 🔗 Additional Resources
- [PostgreSQL Documentation](https://www.postgresql.org/docs/)
- [TypeScript Documentation](https://www.typescriptlang.org/docs/)

## 🔍 Summary
Drizzle simplifies working with PostgreSQL databases. With its easy-to-use commands and configuration, you can manage your data with confidence. Don’t forget to download Drizzle now!

[Download Drizzle Now](https://github.com/amanueln641/Drizzle/releases)