# Installing Xitepress (WordPress) on XAMPP (Windows) and Importing .wpress Backup

This guide provides step-by-step instructions on how to install Xitepress (WordPress) using XAMPP on a Windows environment. Additionally, it explains how to import a .wpress backup file using the WP All in One Migration plugin (mod version) from the provided Git repository.

## Table of Contents
1. [Prerequisites](#prerequisites)
2. [Installing XAMPP](#installing-xampp)
3. [Setting Up the Database](#setting-up-the-database)
4. [Installing Xitepress (WordPress)](#installing-xitepress-wordpress)
5. [Importing .wpress Backup](#importing-wpress-backup)

## Prerequisites
- Windows operating system
- Basic understanding of web technologies
- Git installed on your system

## Installing XAMPP
1. **Download XAMPP:** Go to the [XAMPP website](https://www.apachefriends.org/index.html) and download the Windows version of XAMPP.

2. **Run Installer:** Run the downloaded installer and follow the on-screen instructions. Choose the components you want to install (e.g., Apache, MySQL, PHP, phpMyAdmin).

3. **Start Services:** Once installed, launch XAMPP Control Panel and start the Apache and MySQL services by clicking the "Start" buttons next to them.

## Setting Up the Database
1. **Access phpMyAdmin:** Open a web browser and go to `http://localhost/phpmyadmin/`.

2. **Create Database:** Click on "Databases" in the top menu. Enter a name for your database (e.g., `xitepress`) and click "Create".

## Installing Xitepress (WordPress)
1. **Clone Git Repo:** Open a command prompt or Git Bash and navigate to the directory where you want to clone the repository. Use the following command:
   ```bash
   git clone <repository_url>
   ```

2. **Move Files:** Navigate to the cloned repository directory and move the WordPress files to the appropriate location. For XAMPP, move the files to the `htdocs` folder in your XAMPP installation directory (e.g., `C:\xampp\htdocs\`).

3. **Rename Directory:** Rename the WordPress directory to your preferred name, e.g., `xitepress`.

4. **Access Installation:** Open a web browser and go to `http://localhost/xitepress/` (replace `xitepress` with the chosen directory name).

5. **Complete Installation:** Follow the WordPress installation prompts:
   - Select your language and click "Continue."
   - Enter the database information:
     - Database Name: `xitepress` (or the name you chose)
     - Username: `root`
     - Password: (leave blank)
     - Database Host: `localhost`
     - Table Prefix: (default is fine)
   - Click "Submit" and complete the installation by providing site details and an admin account.

6. **Access WordPress:** After installation, you can access your Xitepress site by going to `http://localhost/xitepress/`.

## Importing .wpress Backup
1. **Install WP All in One Migration (mod version):** The modified version of the plugin with increased upload limits is available in the Git repository. Download the plugin ZIP file from the repository and install it in your WordPress site.

2. **Import Backup:**
   - In the WordPress dashboard, go to "All-in-One WP Migration" > "Import".
   - Upload the `.wpress` backup file (provided in the repository).
   - Follow the prompts to complete the import process.

3. **Verify:** Once the import is successful, verify that your site's content has been correctly restored.

Congratulations! You have successfully installed Xitepress (WordPress) using XAMPP on Windows and imported a .wpress backup using the modified WP All in One Migration plugin.

For further customization and management, refer to the official WordPress documentation.

---
**Note:** Make sure to replace placeholders such as `<repository_url>` with the actual values from your project. This guide assumes a basic understanding of Git, XAMPP, and WordPress concepts.
