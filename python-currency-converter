# currency_converter.py

rates = {
    "USD": 1.0,        # base currency
    "CAD": 1.34,
    "EUR": 0.93,
    "GBP": 0.81,
    "PKR": 284.5
}

print("Welcome to the Currency Converter!")
print("Supported currencies:", ", ".join(rates.keys()))

# Get user input
from_currency = input("Enter the currency you have: ").upper()
to_currency = input("Enter the currency you want: ").upper()
amount = float(input(f"Enter amount in {from_currency}: "))

# Convert
if from_currency in rates and to_currency in rates:
    usd_amount = amount / rates[from_currency]       # convert to USD first
    converted_amount = usd_amount * rates[to_currency]
    print(f"{amount} {from_currency} = {converted_amount:.2f} {to_currency}")
else:
    print("Error: Unsupported currency. Please use the supported codes.")