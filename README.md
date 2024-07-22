## README.md for HealthPass

### HealthPass Overview

HealthPass is a state-of-the-art health management platform designed to transform how medical data is accessed and utilized globally. Our journey began with a critical examination of healthcare inefficiencies in developing countries, particularly in Africa, where inadequate medical record systems significantly lower healthcare standards.

### Table of Contents

- [Installation](#installation)
- [Setting Up the Project](#setting-up-the-project)
- [Project Structure](#project-structure)
- [Working with HTML, CSS, and JavaScript](#working-with-html-css-and-javascript)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

---

### Installation

#### Prerequisites

- **Python**: Ensure Python 3.12 or higher is installed on your machine. You can download it from the [Python Downloads Page](https://www.python.org/downloads/).

#### Installation Steps

1. **Download Python**:
   - Go to the [Python Downloads Page](https://www.python.org/downloads/).
   - Click on the download button for the latest Python version and download the executable installer.

2. **Run the Installer**:
   - Run the downloaded installer.
   - Check the box next to "Install launcher for all users (recommended)" and click "Install Now".

3. **Verify Installation**:
   - Open the command prompt and execute:
     ```bash
     py --version
     ```
   - Ensure the displayed version matches the version you installed.

4. **Install Django**:
   - Create a folder called `summer_hacks`:
     ```bash
     mkdir summer_hacks
     ```
   -  Set up a virtual environment:
     ```bash
     py -m venv healthpass
     healthpass\Scripts\activate.bat
     ```
   - Install Django within the virtual environment:
     ```bash
     py -m pip install Django
     ```

5. **Clone the Repository**:
   - Change directory to your project folder (summer_hacks):
     ```bash
     cd summer_hacks
     git clone https://github.com/H-Badger009/HealthPass.git
     cd HealthPass
     ```

6. **Install Dependencies**:
   - Install the required packages:
     ```bash
     pip install -r requirements.txt
     ```

7. **Run the Django Server**:
   - Check for errors:
     ```bash
     python manage.py check
     ```
   - Start the server:
     ```bash
     python manage.py runserver
     ```
   - Access the application at:
     - [HealthPass](http://127.0.0.1:8000/healthpass/)
     - [Accounts](http://127.0.0.1:8000/accounts/)
     - [Admin](http://127.0.0.1:8000/admin/)

---

### Setting Up the Project

#### Project Structure

- The project consists of two main applications: **healthpass** and **accounts**.
- Each application contains templates and static files necessary for rendering the user interface.

#### Working with HTML, CSS, and JavaScript

1. Navigate to the directory:
   ```bash
   cd summer_hacks\HealthPass\easy_healthcare
   ```

2. Organize your static files:
   - Place CSS files in the `static/styles` folder.
   - Place JavaScript files in the `static/scripts` folder.
   - Place images in the `static/images` folder.

3. In your HTML files, include the following in the `<head>` section:
   ```html
   {% load static %}
   <link rel="stylesheet" type="text/css" href="{% static 'styles/your_style.css' %}">
   <script src="{% static 'scripts/your_script.js' %}"></script>
   ```

---

### Troubleshooting

- If you encounter any issues during setup or execution, ensure that:
  - All dependencies are correctly installed.
  - The virtual environment is activated when running commands.
  - You are using the correct Python version.

---

### Contributing

We welcome contributions to HealthPass! To contribute:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your branch and submit a pull request.

Please ensure your code adheres to the project's coding standards and includes appropriate tests.

---

### License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.