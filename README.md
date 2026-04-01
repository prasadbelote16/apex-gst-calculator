# Oracle APEX GST Calculator

This project demonstrates a GST (Goods and Services Tax) calculator built using Oracle APEX.

## 🚀 Features

- Calculates GST amount based on user input
- Supports GST rates: 5%, 12%, 18%, 28%
- Displays total amount including GST
- Real-time calculation using Dynamic Actions (no button required)

![GST Input](gst_input.png)
![GST Input](gst_input.png)

## 🧠 Logic Used

```plsql
:P5_GST_AMT := (:P5_AMOUNT * :P5_GST) / 100;
:P5_TOTAL := :P5_AMOUNT + :P5_GST_AMT;
