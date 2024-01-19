# Online Course app

## Overview
A Django-based Learning Management System that simulates the online learning experience. Key features are registering users, instructors, students, courses, course lectures, functional online quizes, with django admin.Users are allowed to enroll courses, inspect them and take quizes on site. The web application supports authentication and authorization.

## Getting Started

### Prerequisites

- [Python](https://www.python.org/) installed
- [Pip](https://pip.pypa.io/en/stable/) installed on your machine.

### Running the App

1. Clone this repository to your local machine:

    ```bash
    git clone https://github.com/Li-HsuanChien/Online_course_app.git
    ```

2. Navigate to the project directory:

    ```bash
    cd Online_course_app
    ```

3.  Set up a virtual environment (optional but recommended):

    ```bash
    python -m venv venv
    ```

4. Activate the virtual environment:

    - On Windows:

    ```bash
    venv\Scripts\activate
    ```

    - On Linux/macOS:

    ```bash 
    source venv/bin/activate
    ```

5. Install the required dependencies:

    ```bash
    pip install -U -r requirements.txt
    ```

6. Run the application:

    ```bash
    python manage.py makemigrations
    python manage.py migrate
    python manage.py runserver
    ```
7. The application will be listening to `http://localhost:8000/` by default.

8. Create super user by executing:

    ```bash
    python manage.py createsuperuser
    ```

8. Direct to `http://localhost:8000/admin` to utilize django admin tool to set up courses and users.

9. Direct to `http://localhost:8000/onlinecourse` to use the main application

**Using Docker Containers**

1. Login to Docker Hub:

    - Open a terminal or command prompt and run the following command to log in to Docker Hub:

    ```bash
    docker login
    ```
    - Enter your Docker Hub username and password when prompted.

2. Pull the Online Course App Image:

    - Run the following command to pull the Online Course App Docker image from Docker Hub:

    ```bash
    docker pull shanechien/online_course_app
    ```

3. Run the Container:

    - Once the image is successfully pulled, you can run a container using the following command:
    
    ```bash
    docker run -p 8000:8000 shanechien/online_course_app
    ```
4. The application will be listening to `http://localhost:8000/` by default.

5. Create super user by executing:

    ```bash
    python manage.py createsuperuser
    ```

6. Direct to `http://localhost:8000/admin` to utilize django admin tool to set up courses and users.

7. Direct to `http://localhost:8000/onlinecourse` to use the main application

## Usage
  **Course Management:**
  
  -Add and customize courses with details such as name, description, duration, and prerequisites.
  -Organize course lectures, allowing instructors to upload multimedia content and presentations.

  **Quiz Hosting:**

    -Utilize Django Admin features to create and manage quizzes with varying complexities.
    -Define quiz parameters, set answers, grade values, with diverse question types, then calulate results when submitted.
    -Allow reviewing right and wrong answers.

**User Authentication and Roles:**

    -Robust authentication mechanisms ensure secure access with customizable user roles.


## Awaiting Updates

**Role focused functions**
    
    -Allow instructors to give feedback, grading, and other features
    -Provide to learners User-friendly dashboards provide information on enrolled courses, upcoming lectures, and assessment deadlines.

**Customization Options:**

    Tailor the platform to your institution's branding with customizable themes and logos.
    Integration capabilities with external systems for a seamless learning ecosystem.

**Scalability and Performance:**

    -Hosting independent sites and data base with cloud, ensuring scalability for growing user bases.
    -Robust performance optimization guarantees a smooth and responsive experience.

## Contributing

Feel free to contribute to the development of this budget management system by creating issues or pull requests.

## License

This project is licensed under the Apache 2.0 - see the [LICENSE](LICENSE) file for details.
