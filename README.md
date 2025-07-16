# SmartCart – Python-Based Retail Billing & Payment System

SmartCart is a Python-based interactive retail billing system built using Google Colab. It simulates real-world shopping cart functionality including barcode-based product addition, billing, UPI QR code generation, payment verification via UTR codes, and a customer feedback system.

## Features

- Scan/add items using barcodes (from a CSV-based product list)
- Maintain a cart and dynamically calculate totals
- Auto-apply discounts as defined per product
- Generate a UPI QR code for payment
- Verify UTR number against a predefined CSV
- Store bills in Google Drive as text files
- Collect star ratings and textual feedback from customers

## Technologies Used

- Python
- SQLite (in-memory)
- Pandas
- qrcode
- ipywidgets (interactive UI)
- PIL (image display)
- Google Colab + Drive for storage

## File Structure
smartcart/
├── products.csv # List of products with barcodes
├── UTR.csv # List of valid UTR codes
├── store.db # SQLite database (created on runtime)
├── SmartCart.ipynb # Main notebook
├── /SmartCart_Bills/ # Google Drive folder to store bills
## How to Run

1. Open the notebook in Google Colab.
2. Upload your `products.csv` and `UTR.csv` or link them from Drive.
3. Run the notebook cells step by step.
4. Enter barcodes to add items to cart.
5. Click "Generate Payment QR" to create a UPI QR code.
6. Enter UTR code to verify payment.
7. Download bill from Drive and submit feedback.

## Sample `products.csv` Format

