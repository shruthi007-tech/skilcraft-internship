def celsius_to_fahrenheit(c):
    return (c * 9/5) + 32

def celsius_to_kelvin(c):
    return c + 273.15

def fahrenheit_to_celsius(f):
    return (f - 32) * 5/9

def fahrenheit_to_kelvin(f):
    return (f - 32) * 5/9 + 273.15

def kelvin_to_celsius(k):
    return k - 273.15

def kelvin_to_fahrenheit(k):
    return (k - 273.15) * 9/5 + 32

print("Temperature Converter")
print("1. Celsius to Fahrenheit and Kelvin")
print("2. Fahrenheit to Celsius and Kelvin")
print("3. Kelvin to Celsius and Fahrenheit")

choice = int(input("Enter your choice (1-3): "))

if choice == 1:
    c = float(input("Enter temperature in Celsius: "))
    print("Fahrenheit:", celsius_to_fahrenheit(c))
    print("Kelvin:", celsius_to_kelvin(c))
elif choice == 2:
    f = float(input("Enter temperature in Fahrenheit: "))
    print("Celsius:", fahrenheit_to_celsius(f))
    print("Kelvin:", fahrenheit_to_kelvin(f))
elif choice == 3:
    k = float(input("Enter temperature in Kelvin: "))
    print("Celsius:", kelvin_to_celsius(k))
    print("Fahrenheit:", kelvin_to_fahrenheit(k))
else:
    print("Invalid choice. Please enter 1, 2 or 3.")
