# 🤖 DecodeLabs Prompt Engineering Project 1

## 👨‍🎓 Student Information
- **Name:** Patel Dwij Jatinkumar  
- **Batch:** 2026  
- **Project:** Zero-Shot & Few-Shot Data Extraction  

---

## 🎯 Objective
Design a prompt that converts unstructured text into structured JSON output using delimiters, few-shot examples, and strict formatting rules.

---

## 📌 Problem Statement
Extract the following fields from messy text:
- Name  
- Email  
- Phone  
- City  
- Occupation  

Return output in **valid JSON format only**.

---

## 🧠 Final Prompt

You are a Data Extraction AI.

### ⚙️ Rules:
1. Extract **Name, Email, Phone, City, and Occupation**.
2. Return **ONLY valid JSON**.
3. Do not add explanations.
4. If any data is missing, return `null`.
5. Follow the examples exactly.

---

## 📖 Example Input
My name is Rahul Sharma.
I live in Ahmedabad.
My email is rahul@gmail.com
I work as a Software Engineer.
Phone: 9876543210
---

## 🧪 Test Case

### Input
Hi, I am Dwij Patel.
I study Computer Engineering.
My email is dwijjpatel09@gmail.com
I live in Mehsana.
Phone Number: 9313716613

---

## ✅ Output
```json
{
  "name": "Dwij Patel",
  "email": "dwijjpatel09@gmail.com",
  "phone": "9313716613",
  "city": "Mehsana",
  "occupation": "Computer Engineering Student"
}
