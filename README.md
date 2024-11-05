# Inventory-Management-web-app-using-Flask

## Overview

The **Flask Inventory Management App** is a simple and efficient web application built using Flask, designed for managing the inventory, purchases, and sales operations for small businesses. This application helps users track items, manage quantities, handle purchases, and process sales with automatic updates to stock levels and cash balance.

## Features

- **Item Management**: Add, update, and view items in the inventory.
- **Purchases Module**: Track purchases, adjust stock levels, and manage purchase history.
- **Sales Module**: Process sales, reduce item quantities, and update cash balance.
- **Detailed History**: Keep track of all purchase and sales transactions.
- **Real-Time Cash Balance**: View the company’s current cash balance updated after each transaction.
- **User-Friendly Interface**: Simple, intuitive interface to streamline inventory management tasks.

## Technologies Used

- **Backend**: Flask (Python)
- **Database**: SQLite
- **Frontend**: HTML, CSS
- **Deployment**: GitHub and LinkedIn integration for project showcasing

## Setup and Installation

Follow these steps to set up the project locally:

### Prerequisites

- Python 3.x
- Flask (`pip install flask`)
- SQLite (for database management)

### Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/Flask-Inventory-Management-App.git
    cd Flask-Inventory-Management-App
    ```

2. **Install Required Packages**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Initialize Database**:
   Set up the SQLite database by running:
    ```bash
    python initialize_db.py
    ```
   This will create the necessary tables for storing item data, purchase and sales history, and cash balance.

4. **Run the Application**:
    ```bash
    flask run
    ```
   Access the application at `http://127.0.0.1:5000`.

## Usage

1. **Home Page**:
   - View current cash balance.
   - Access buttons for managing items, purchases, and sales.

2. **Item Management**:
   - Navigate to **Add Item** to add new items to the inventory.
   - Select **Edit Item** to update item details or adjust quantities.

3. **Purchases**:
   - Enter item ID, quantity, and rate to record a purchase.
   - View **Purchase History** to see past transactions and stock adjustments.

4. **Sales**:
   - Select items and input quantity and rate to process a sale.
   - The sales amount is added to the cash balance, and inventory quantities are updated.


## Project Structure

```plaintext
Flask-Inventory-Management-App/
├── app.py                 # Main application code
├── templates/             # HTML templates
│   ├── index.html         # Home page
│   ├── add_item.html      # Add item page
│   ├── edit_item.html     # Edit item page
│   ├── purchase.html      # Purchase page
│   └── sales.html         # Sales page
├── static/                # Static files (CSS, JS, images)
│   └── index.css          # Main stylesheet
├── initialize_db.py       # Script to initialize the database
├── README.md              # Project documentation
└── requirements.txt       # List of dependencies
