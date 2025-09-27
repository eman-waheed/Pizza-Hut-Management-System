Pizza Hut Management System

Overview
This project is a web-based Pizza Ordering System that allows clients to place pizza orders, 
submit feedback, and view their order history, while administrators can manage orders and monitor 
customer feedback. The system is implemented using PHP, MySQL, HTML, and CSS, and runs on a local 
XAMPP server. It demonstrates key concepts of full-stack web development including authentication, 
role-based access, SQL integration, and secure coding practices.

Objectives
- Provide an online pizza ordering experience for clients
- Allow secure client registration, login, and feedback
- Enable administrators to view/manage orders and customer reviews
- Demonstrate database-driven web development using PHP and MySQL

Features
- User Registration and Login (Clients/Admin)
- Client Dashboard with order form, reviews, and site statistics
- Admin Dashboard with order management and feedback monitoring
- Secure login with hashed passwords
- Role-based access control (Client/Admin)
- Order history with payment method integration
- SQL JOIN queries for combining relational data
- Data validation and error handling

Tech Stack
- Frontend: HTML5, CSS3
- Backend: PHP
- Database: MySQL
- Server: XAMPP (Apache, MySQL)
- IDE: Visual Studio Code

Database Design
- customers (customer_id, name, phone, address, email, password, created_at)
- orders (order_id, customer_id, order_date, status, total_amount)
- order_details (detail_id, order_id, pizza_id, quantity, price, size)
- pizzas (pizza_id, name, size, crust, price, available)
- feedback (feedback_id, customer_id, order_id, rating, comment, created_at)
- payments (payment_id, order_id, amount, payment_method, payment_date)
- users (user_id, username, password, role, full_name, email, phone)

Security Measures
- Passwords hashed using PHP password_hash()
- SQL Injection prevention via prepared statements
- Session-based authentication with role validation
- Form input validation (HTML + PHP filters)

Files in this Repository
- Report.pdf : Detailed project documentation
- index.php : Home page with login and registration links
- login.php / register.php : User authentication
- home.php : Client dashboard
- admin_panel.php : Admin dashboard
- order.php : Order form with payment integration
- admin_orders.php : Admin order management
- feedback.php / view_feedback.php : Feedback handling
- Database.sql : Database schema and table creation scripts

Future Enhancements
- Add real online payment gateway integration
- Add more pizza customization options
- Mobile responsive design for better user experience
- Cloud deployment (Heroku, AWS, or cPanel hosting)
