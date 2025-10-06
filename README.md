# Inventory Management System


## Installation & Setup

### Prerequisites

- Python 3.8 or higher
- pip (Python package manager)

### Step 1: Clone or Download

```bash
# If using git
git clone <repository-url>
cd inventory_system
```

### Step 2: Create Virtual Environment (Recommended)

```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate

# On macOS/Linux:
source venv/bin/activate
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Run the Application

```bash
python app.py
```

## Sample Data

The application comes pre-loaded with sample data:

### Products (4 items)
- Laptop Dell XPS 15
- Wireless Mouse Logitech
- USB-C Cable
- Monitor Samsung 27"

### Locations (4 warehouses)
- Main Warehouse (New York)
- Retail Store Downtown (New York)
- Distribution Center East (Newark)
- Regional Hub West (Los Angeles)

### Movements (20 transactions)
- Initial stock arrivals
- Transfers between locations
- Sales/outgoing transactions
- Restocking operations

## Usage Guide

### Managing Products

1. **View Products**: Click "Products" in the navigation menu
2. **Add Product**: Click "Add New Product" button
   - Enter product name (required)
   - Add description (optional)
   - Click "Save Product"
3. **Edit Product**: Click "Edit" button next to any product
4. **Delete Product**: Click "Delete" button (only if no movements exist)

### Managing Locations

1. **View Locations**: Click "Locations" in the navigation menu
2. **Add Location**: Click "Add New Location" button
   - Enter location name (required)
   - Add address (optional)
   - Click "Save Location"
3. **Edit Location**: Click "Edit" button next to any location
4. **Delete Location**: Click "Delete" button (only if no movements exist)

### Managing Product Movements

1. **View Movements**: Click "Movements" in the navigation menu
2. **Add Movement**: Click "Add New Movement" button
   - Select product (required)
   - Select from location (optional - leave empty for incoming)
   - Select to location (optional - leave empty for outgoing)
   - Enter quantity (required, must be > 0)
   - Click "Save Movement"
3. **Edit Movement**: Click "Edit" button next to any movement
4. **Delete Movement**: Click "Delete" button

### Viewing Reports

1. Click "Reports" in the navigation menu
2. View inventory balance for each product in each location
3. Green badges indicate positive stock
4. Red badges indicate negative stock (potential data errors)
5. Only locations with non-zero balance are displayed



## Technologies Used

- **Backend**: Flask 3.0.0
- **ORM**: Flask-SQLAlchemy 3.1.1
- **Database**: SQLite
- **Frontend**: Bootstrap 5.3.0
- **Icons**: Bootstrap Icons 1.11.0
- **Python**: 3.8+

