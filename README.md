# Online Course CBT Platform

A comprehensive Online Course platform with Computer-Based Testing (CBT) functionality, developed using Laravel and Tailwind CSS. This application allows users to enroll in various courses, take quizzes, track their progress, and view results. It’s designed for students and administrators, with a user-friendly interface and extensive course and question management options.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## Features

### For Students
- **Course Enrollment**: Enroll in available courses.
- **CBT Functionality**: Take quizzes and answer multiple-choice questions.
- **Progress Tracking**: Track completion status for each course.
- **Results View**: View test results, including pass/fail status.

### For Admins
- **Course Management**: Add and manage courses and categories.
- **Question Management**: Add, update, or delete questions associated with courses.
- **Student Progress Monitoring**: View each student’s progress and test results.

## Installation

To get this project up and running on your local machine, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/online-course-cbt-platform.git
   cd online-course-cbt-platform
   ```

2. **Install Dependencies**:
   Make sure you have [Composer](https://getcomposer.org/) and [Node.js](https://nodejs.org/) installed. Then, run:
   ```bash
   composer install
   npm install
   ```

3. **Environment Configuration**:
   Copy `.env.example` to `.env`:
   ```bash
   cp .env.example .env
   ```
   Update `.env` with your database and mail configurations.

4. **Generate Application Key**:
   ```bash
   php artisan key:generate
   ```

5. **Run Migrations and Seed the Database**:
   ```bash
   php artisan migrate --seed
   ```

6. **Compile Assets**:
   ```bash
   npm run dev
   ```

## Configuration

1. **Database**: Configure your database credentials in the `.env` file.
2. **Mail**: Set up your email credentials to enable notifications (optional).

## Usage

To start the server, run:
```bash
php artisan serve
```
Visit the application at `http://localhost:8000` in your browser.

### Navigating the Application

- **Student Dashboard**: View enrolled courses, track progress, and take quizzes.
- **Admin Dashboard**: Manage courses, questions, and student progress.

## Technologies Used

- **Laravel 11**: Backend framework.
- **Tailwind CSS**: For responsive and modern design.
- **MySQL**: Database.
- **Blade**: Templating engine for front-end.

## Folder Structure

- **app/Http/Controllers**: Contains controllers for handling business logic.
- **resources/views**: Blade views for rendering the front-end.
- **public**: Contains public assets like images and CSS.
- **routes**: Contains application routes (`web.php`).

## Contributing

If you’d like to contribute to this project, please fork the repository and use a feature branch. Pull requests are warmly welcome.

1. Fork the repository.
2. Create a new branch with a descriptive name.
3. Make your changes and commit them.
4. Open a pull request.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
