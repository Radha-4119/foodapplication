# Online Python compiler (interpreter) to run Python online.
# Write Python 3 code in this online editor and run it.
# Define some menu items
menu = {
    "Appetizers": {
        "Calamari": 12.99,
        "Bruschetta": 8.50,
        "Soup of the Day": 5.95
    },
    "Main Courses": {
        "Spaghetti Carbonara": 16.75,
        "Grilled Chicken Breast": 18.25,
        "New York Strip Steak": 24.50
    },
    "Desserts": {
        "Tiramisu": 7.25,
        "Chocolate Cake": 6.95,
        "Ice Cream": 4.50
    }
}

# Function to print a menu section with a separator
def print_menu_section(section_name):
  print(f"\n{section_name.upper()}")
  print("-" * len(section_name))
  for item, price in menu[section_name].items():
    print(f"{item:<25} ${price:.2f}")

# Print the entire menu
for section in menu:
  print_menu_section(section)
