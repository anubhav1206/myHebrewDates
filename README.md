# My Hebrew Dates

Certainly! Here's an example of an "About the Project" section you can include for the MyHebrewDates web app:

---

## About the Project

MyHebrewDates is a web application designed to facilitate the sharing and management of Hebrew dates such as birthdays, anniversaries, and yahrzeits. The app provides a user-friendly platform for individuals and communities to keep track of important Hebrew dates and ensure they are never missed.

### Key Features

- **Hebrew Date Management:** Users can easily add and manage Hebrew dates important to them, such as birthdays, anniversaries, and yahrzeits. The app provides a convenient interface for inputting Hebrew dates and associating them with relevant information.

- **Subscribable Calendar Feed:** MyHebrewDates offers a subscribable feed that integrates seamlessly with popular calendar applications. Users can subscribe to the feed and receive automatic updates and reminders about upcoming Hebrew dates directly in their preferred calendar app.

- **User Accounts and Notifications:** The app supports user accounts, allowing individuals to create personalized profiles and manage their Hebrew date preferences. Users can choose to receive email or push notifications to ensure they never miss an important Hebrew date.

- **Collaborative Sharing:** MyHebrewDates enables users to share Hebrew dates with family members, friends, or communities. Users can invite others to join events and synchronize Hebrew dates across multiple calendars, fostering a sense of connection and collaboration.

### Technologies Used

The MyHebrewDates web app is built using modern web development technologies. The key technologies and frameworks used in the project include:

- Python and Django: The backend of the app is powered by Python, utilizing the Django web framework for efficient and scalable development.

- JavaScript and React: The frontend interface is built using JavaScript and the React library, providing a responsive and interactive user experience.

- Celery: The app employs Celery, a distributed task queue system, to handle background tasks and asynchronous processing.

- PostgreSQL: The project utilizes PostgreSQL as the relational database management system to store and manage data efficiently.

To set up the MyHebrewDates web app locally, you can follow the instructions provided in the readme file. Here's a breakdown of the steps involved:

3. **Setting Up Your Users:**
   - To create a normal user account, go to the "Sign Up" page and fill out the form. After submission, you'll see a "Verify Your E-mail Address" page. Check your console to find a simulated email verification message and click on the link to verify the user's email.
   - To create a superuser account (admin account), use the following command in your terminal:
     ```
     $ python manage.py createsuperuser
     ```
     Follow the prompts to set a username and password for the superuser.

a. **Type Checks:**
   - You can run type checks using MyPy with the following command:
     ```
     $ mypy my_hebrew_dates
     ```

b. **Test Coverage:**
   - To run the tests and check the coverage, use the following commands:
     ```
     $ coverage run -m pytest
     $ coverage html
     ```
     This will generate an HTML coverage report, which you can view by opening the `htmlcov/index.html` file in your browser.

c. **Running Tests with Pytest:**
   - You can run the tests using Pytest by running the following command:
     ```
     $ pytest
     ```

5. **Live Reloading and Sass CSS Compilation:**
   - Follow the instructions provided in the [Live reloading and Sass compilation](https://cookiecutter-django.readthedocs.io/en/latest/developing-locally.html#sass-compilation-live-reloading) section to set up live reloading and Sass CSS compilation.

6. **Celery:**
   - MyHebrewDates uses Celery for background task processing. To run a Celery worker, use the following command:
     ```
     $ cd my_hebrew_dates
     $ celery -A config.celery_app worker -l info
     ```
     Make sure you are in the same folder as `manage.py` for the Celery commands to work correctly.
   - If you need to run periodic tasks, you can start the Celery beat scheduler service using either of the following commands:
     - Standalone process:
       ```
       $ cd my_hebrew_dates
       $ celery -A config.celery_app beat
       ```
     - Embedding beat service inside a worker (not recommended for production):
       ```
       $ cd my_hebrew_dates
       $ celery -A config.celery_app worker -B -l info
       ```

These are the basic steps to set up and run the MyHebrewDates web app locally. Make sure to check the provided documentation for any additional details or specific configurations required for your environment.****  

### Credits and Contributors

The development of the MyHebrewDates web app has been made possible by the contributions of a talented team of developers and contributors. We extend our appreciation to the following individuals who have dedicated their time and expertise to this project:

- [Abe Hanoka]


We express our gratitude to each of these individuals for their valuable contributions and commitment to creating a reliable and user-friendly platform for managing Hebrew dates.

---


