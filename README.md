# Serein: Django E-Commerce Platform


## Overview of the Project
This project is a functional e-commerce platform prototype built using the Django framework. The objective was to design a technical solution for a retail platform, applying subject concepts such as modular web development, database management, and asynchronous client-side scripting. The system is designed to provide customers with a seamless experience for browsing products and managing purchases.

## Features
The project incorporates several specific features and functional modules. Following the requirement for the project, the system includes:

1.  **User Management:**
    *   User registration, login, and authentication.
    *   User profile views and basic management (aligned with the 'User management' example requirement) [4].

2.  **Product Catalog & Display (Data Input & Processing):**
    *   **CRUD** (Create, Read, Update, Delete) capabilities for managing product inventory via an admin interface [4].
    *   Displaying products with descriptions, pricing, and images.
    *   Utilizing **Owl Carousel** for dynamic, responsive image sliders on the homepage/product detail pages.

3.  **Shopping Cart & Checkout Workflow:**
    *   A clear logical workflow for the user to interact with the system.
    *   Ability for authenticated users to add items to a shopping cart, view cart contents, and adjust quantities.
    *   Simulated checkout process to finalize an order.

### Non-Functional Considerations
The design included considerations for non-functional requirements, such as:
*   **Usability:** Ensuring a clear and intuitive user interface using HTML, CSS, and JavaScript.
*   **Maintainability:** Utilizing Django's modular app structure for clean implementation.
*   **Error Handling:** Implementing validation checks for user input and graceful failure handling.

## Technologies/Tools Used
This project was developed using a standard web stack leveraging Python and Django [1].

[| Component | Technology | Role |]
| **Backend Framework** | Django (Python) | Server-side logic, routing, template rendering, ORM |
| **Programming Language** | Python | Primary development language |
| **Database** | dbsqlite (SQLite) | Default development database for persistence and storage |
| **Frontend** | HTML, JavaScript, CSS | Markup, client-side interactivity, and styling |
| **Libraries** | Owl Carousel | Used for responsive product display carousels/sliders |
| **Version Control** | Git / GitHub | Used for tracking changes and submission [1, 3] |

## Steps to Install & Run the Project

The steps below assume you have Python 3 and Git installed on your machine.

### 1. Clone the Repository
```bash
git clone [https://github.com/Parth-Malguri/Parth-VITyarthi-project/tree/main]
cd MyDjangoShop
(Note: Version control usage (Git) is a key technical expectation for the submission).
2. Set up the Environment
Create and activate a Python virtual environment:
python -m venv venv
venv\Scripts\activate   
3. Install Dependencies
Install all required Python packages (e.g., Django):
pip install django
pip install pillow
pip install mysqlclient
4. Database Setup
The project uses SQLite. Apply migrations to create the necessary database schema:
python manage.py makemigrations
python manage.py migrate
5. Create Superuser (Optional, for Admin Access)
To access the Django Admin panel for product management (CRUD operations):
python manage.py createsuperuser
6. Run the Server
Start the local development server:
python manage.py runserver
The application will now be accessible at http://127.0.0.1:8000/.
Instructions for Testing
To validate the functionality of the e-commerce platform, follow these steps:
1. User Flow Validation: Register a new user and confirm successful login. Attempt to access restricted pages (e.g., the checkout step) before logging in to verify Security and Error handling.
2. Product Interaction: Browse the homepage and product detail pages. Test the Owl Carousel responsiveness.
3. Order Placement: Proceed through the simulated checkout process, confirming the final order details are displayed correctly.
4. Admin Testing: Log into the /admin interface using the superuser credentials. Validate that new products can be created, updated, and deleted (CRUD operations).
