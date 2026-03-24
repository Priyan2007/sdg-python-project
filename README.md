# sdg-python-project
# 🌿 Carbon Footprint Calculator (SDG 13)

## 📌 Project Overview

This project is a **Python-based Carbon Footprint Calculator** developed as part of Sustainable Development Goals (**SDG 13: Climate Action**).

It helps users estimate their **daily carbon dioxide (CO₂) emissions** based on:

* 🚗 Travel habits
* ⚡ Electricity usage
* 🍽️ Food consumption

The project also provides **suggestions to reduce carbon footprint** and promote an eco-friendly lifestyle.

---

## 🎯 Objectives

* To create awareness about carbon emissions
* To help users monitor their daily environmental impact
* To encourage sustainable living practices

---

## 🛠️ Technologies Used

* Python
* VS Code

---

## ⚙️ Features

* Calculates carbon emission from:

  * Travel (car, bus, bike)
  * Electricity consumption
  * Food habits (veg / non-veg)
* Displays total CO₂ emission per day
* Provides environmental suggestions
* Simple and user-friendly interface (console-based)

---

## ▶️ How to Run the Project

1. Open the project in **VS Code**
2. Open terminal
3. Run the following command:

```
python main.py
```

---

## 🧪 Sample Input

```
Enter daily travel distance (in km): 10  
Mode of transport (car/bus/bike): car  
Enter electricity usage (kWh): 5  
Food type (veg/non-veg): non-veg  
```

---

## 📊 Sample Output

```
🌍 --- Carbon Footprint Report ---
Total CO2 emission: 8.60 kg/day
👍 Moderate impact. Try to reduce more.

💡 Suggestions to reduce footprint:
- Use public transport
- Save electricity
- Prefer plant-based food
- Avoid plastic usage
```

---

## 🌱 Future Enhancements

* Add Graphical User Interface (GUI) using Tkinter
* Store user data using files or database
* Display charts using Matplotlib
* Convert into a web/mobile application

---

## 🌍 SDG Goal

This project supports **Sustainable Development Goal 13: Climate Action**, focusing on reducing environmental impact and spreading awareness.

---
PROGRAM:
```
# Carbon Footprint Calculator (SDG 13)

def calculate_travel_emission():
    km = float(input("Enter daily travel distance (in km): "))
    mode = input("Mode of transport (car/bus/bike): ").lower()

    if mode == "car":
        return km * 0.21
    elif mode == "bus":
        return km * 0.10
    elif mode == "bike":
        return km * 0.05
    else:
        print("Invalid mode! Assuming car.")
        return km * 0.21


def calculate_electricity_emission():
    units = float(input("Enter daily electricity usage (in kWh): "))
    return units * 0.5


def calculate_food_emission():
    food = input("Food type (veg/non-veg): ").lower()

    if food == "veg":
        return 1.5
    elif food == "non-veg":
        return 3.0
    else:
        print("Invalid input! Assuming veg.")
        return 1.5


def show_result(total):
    print("\n🌍 --- Carbon Footprint Report ---")
    print(f"Total CO2 emission: {total:.2f} kg/day")

    if total < 5:
        print("✅ Excellent! You are eco-friendly.")
    elif total < 10:
        print("👍 Moderate impact. Try to reduce more.")
    else:
        print("⚠️ High carbon footprint! Take action.")

    print("\n💡 Suggestions to reduce footprint:")
    print("- Use public transport")
    print("- Save electricity")
    print("- Prefer plant-based food")
    print("- Avoid plastic usage")


def main():
    print("🌿 Carbon Footprint Calculator 🌿")

    travel = calculate_travel_emission()
    electricity = calculate_electricity_emission()
    food = calculate_food_emission()

    total = travel + electricity + food

    show_result(total)


# Run program
main()
```

OUTPUT:

<img width="597" height="396" alt="Screenshot 2026-03-24 183054" src="https://github.com/user-attachments/assets/6f731aa5-e06c-444a-bf19-e1fe8f322e8a" />

RESULT:

The project demonstrates how programming can be used to address real-world environmental issues.
It helps create awareness about climate change and encourages users to adopt eco-friendly habits.




