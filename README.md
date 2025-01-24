
# KeepLite

KeepLite is a lightweight, simple, and secure note-taking application built using the LAMP stack (Linux, Apache, MySQL, PHP). It offers essential CRUD (Create, Read, Update, Delete) functionality for managing notes, with a focus on simplicity, performance, and scalability. The application is designed to be responsive and lightweight, making it ideal for low-end systems and quick access to personal notes.

## Features

- **User Authentication**: Secure login and password management with encryption and hashing.
- **Note Management**: Create, edit, categorize, and archive notes.
- **Mind Mapping**: Visualize your thoughts with mind maps (optional).
- **Dark/Light Mode**: Switch between dark and light themes for comfort.
- **Customization**: Toggle app features on/off via settings.
- **Simple, Responsive UI**: A minimalist design optimized for performance on low-end systems.

## Installation

To get started with KeepLite, follow these steps:

### Prerequisites

1. A LAMP stack environment (Linux, Apache, MySQL, PHP).
2. Composer (for managing dependencies).
3. A local server environment like XAMPP or MAMP can also be used.

### Steps

1. Clone the repository:

   ```bash
   git clone https://github.com/terrylan/KeepLite.git
   ```

2. Navigate to the project directory:

   ```bash
   cd KeepLite
   ```

3. Set up the database:

   - Create a new database in MySQL (e.g., `keeplite_db`).
   - Import the schema found in `database/keeplite_schema.sql`.

4. Configure your environment:

   - Edit the `config.php` file to match your database credentials.
   - Make sure the Apache server has write permissions for the `uploads` and `logs` directories.

5. Access the application:

   - Open your browser and navigate to `http://localhost/keeplite`.

6. Follow the on-screen instructions to complete the setup.

## Technologies Used

- **PHP**: Server-side scripting language for app logic.
- **MySQL**: Database for storing user data and notes.
- **HTML/CSS**: Front-end design and structure.
- **JavaScript**: For UI interactions and responsiveness.
- **Bootstrap**: For mobile-first responsive design.
- **bcrypt**: For password hashing and security.

## Features to be Added

- **Tags for Notes**: Categorize notes with custom tags.
- **Collaborative Notes**: Share and collaborate on notes with other users.
- **Export Notes**: Export notes to formats like PDF or text files.
- **Backup and Restore**: Option for users to back up and restore their notes.

## Security

- Passwords are securely hashed using **bcrypt** before being stored in the database.
- The app uses **prepared statements** to prevent SQL injection attacks.
- Data can be encrypted before storage for extra security (optional).

## Contribution

Feel free to fork this repository and submit pull requests. Contributions are welcome! Please follow the standard GitHub workflow:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
