# ⚡ Electricity Bill Calculator

A simple Python program to calculate electricity bills based on tiered unit consumption rates.

---

## 📋 Description

This program takes the number of electricity units consumed as input and calculates the total bill based on a slab-rate pricing system. Different unit ranges are charged at different rates, which is a common billing model used by electricity boards.

---

## 💡 Slab Rate Structure

| Units Consumed | Rate per Unit |
|----------------|---------------|
| 0 – 100 units  | ₹1.50         |
| 101 – 200 units | ₹2.50        |
| 201 – 300 units | ₹4.00        |
| Above 300 units | ₹6.00        |

> Each slab is charged only for the units that fall within that range (progressive billing).

---

## 🚀 How to Run

**Prerequisites:** Python 3.x installed on your system.

**Steps:**

```bash
# Clone the repository
git clone https://github.com/your-username/electricity-bill-calculator.git

# Navigate into the folder
cd electricity-bill-calculator

# Run the script
python electricity_bill.py
```

**Example:**

```
Enter electricity units consumed: 250
Electricity Bill = ₹775.00
```

**Calculation breakdown for 250 units:**
- First 100 units → 100 × ₹1.50 = ₹150.00
- Next 100 units → 100 × ₹2.50 = ₹250.00
- Remaining 50 units → 50 × ₹4.00 = ₹200.00
- **Total = ₹600.00**

---

## 📂 Project Structure

```
electricity-bill-calculator/
│
└── electricity_bill.py    # Main Python script
└── README.md              # Project documentation
```

---

## 🛠️ Technologies Used

- **Language:** Python 3
- **Concepts:** Conditional statements (`if-elif-else`), user input, string formatting

---

## 📌 Features

- Interactive command-line input
- Accurate slab-based (progressive) billing
- Displays bill rounded to 2 decimal places
- Lightweight — no external libraries required

---

## 🤝 Contributing

Pull requests are welcome! If you'd like to improve this project (e.g., add a GUI, include fixed charges, or support multiple months), feel free to fork the repository and submit a PR.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
