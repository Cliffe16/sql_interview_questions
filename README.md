#  LuxDevHQ SQL LeetCode Challenge

Welcome to the **LuxDevHQ SQL LeetCode Challenge**.

Get ready to level up your SQL skills with a mix of real-world problem-solving and LeetCode-style challenges.

This session is designed to strengthen your understanding of:

- SQL Joins  
- Aggregations  
- Window Functions  
- Data Manipulation Techniques  

We’ll start with a sample query problem to warm up, then dive into hands-on LeetCode challenges covering beginner to intermediate-level SQL concepts.

Remember to think critically, write clean queries, and collaborate with your peers — it’s all about learning and growing together! 🚀

---

Linking records across several datasets is important when dealing with health data at the Commission.  

Sometimes patient information must be matched approximately using shared attributes such as:

- Age  
- Sex  
- Birth Date  
- Race/Ethnicity  
- ZIP Code  

Suppose vaccination information was split among **three tables**, each using different patient IDs and with **no direct mapping between them**.

---

## 🏥 Vaccination Clinic 1  
**Table Name:** `clinic1_data`

| PatientID | PatientAge | PatientSex | RACE_ETH | PatientZIP | VaccineType | VacsDate |
|------------|------------|------------|-----------|------------|-------------|------------|
| 20182749 | 28 | F | WHITE | 02118 | 3 | 01032024 |
| 22837162 | 56 | M | BLACK | 02119 | 4 | 01032024 |
| 22832861 | 58 | M | BLACK | 02110 | 4 | 01032024 |
| ... | ... | ... | ... | ... | ... | ... |

---

## 🏥 Vaccination Clinic 2  
**Table Name:** `clinic2_data`

| PtID | AGE | PTSEX | RACETHCODE | ZIPCODE | VaccClass | DATE_OF_VA |
|------|-----|--------|------------|----------|------------|-------------|
| 9847271 | 28 | F | WHITE | 02118 | 2 | 16122024 |
| 6289398 | 56 | M | BLACK | 02119 | 2 | 16122024 |
| 2638928 | 58 | M | BLACK | 02110 | 3 | 16122024 |
| ... | ... | ... | ... | ... | ... | ... |

---

## 🏥 Vaccination Clinic 3  
**Table Name:** `clinic3_data`

| PatID | AGE | PTSEX | RACETHCODE | ZIPCODE | VaccClass | DATE_OF_VA |
|--------|-----|--------|------------|----------|------------|-------------|
| A83719DH | 28 | F | WHITE | 02118 | 2 | 24112023 |
| BIBDSJFQ | 56 | M | BLACK | 02119 | 2 | 24112023 |
| FXV9281X | 58 | M | BLACK | 02110 | 3 | 24112023 |
| ... | ... | ... | ... | ... | ... | ... |

---

## 🧩 Your Task

Since the patient identifiers differ across all three datasets, construct a SQL query that:

- Matches patients approximately using:
  - Age  
  - Sex  
  - Race/Ethnicity  
  - ZIP Code  
- Merges vaccination data across all clinics
- Returns a unified vaccination history
- Includes:
  - `PatientID` (from `clinic1_data`)
  - `PatientAge`
  - `PatientSex`
  - `PatientZIP`
  - `VaccineType`
  - `VaccineDate`

You may use any SQL dialect (PostgreSQL, MySQL, MSSQL, etc.) and make reasonable assumptions where necessary.

---


##  Sample Question 1

Using the 3 tables:

- `clinic1_data`
- `clinic2_data`
- `clinic3_data`

Construct a SQL query (any dialect — Postgres, MariaDB, MSSQL, etc.) that:

- Matches patient information based on:
  - Age  
  - Sex  
  - Race/Ethnicity  
  - Zipcode  
- Makes reasonable assumptions about which columns map to each other  
- Returns merged vaccination data for different dates  

### Required Output Columns:

- `PatientID` (from `clinic1_data`)
- `PatientAge`
- `PatientSex`
- `PatientZIP`
- `VaccineType`
- `VaccineDate`

---

#  Workshop Challenge Questions

1. **Challenge 627. Swap Salary**  
   https://leetcode.com/problems/swap-salary/description  

2. **Challenge 1321. Restaurant Growth**  
   https://leetcode.com/problems/restaurant-growth/description  

3. **Challenge 1873. Calculate Special Bonus**  
   https://leetcode.com/problems/calculate-special-bonus/description  

4. **Challenge 1978. Employees Whose Manager Left the Company**  
   https://leetcode.com/problems/employees-whose-manager-left-the-company/description  

5. **Challenge 1890. The Latest Login in 2020**  
   https://leetcode.com/problems/the-latest-login-in-2020/description  

6. **Challenge 601. Human Traffic of Stadium**  
   https://leetcode.com/problems/human-traffic-of-stadium/description  

7. **Challenge 185. Department Top Three Salaries**  
   https://leetcode.com/problems/department-top-three-salaries/description  

8. **Challenge 570. Managers with at Least 5 Direct Reports**  
   https://leetcode.com/problems/managers-with-at-least-5-direct-reports/description  

9. **Challenge 1045. Customers Who Bought All Products**  
   https://leetcode.com/problems/customers-who-bought-all-products/description  

10. **Challenge 1158. Market Analysis I**  
    https://leetcode.com/problems/market-analysis-i/description  
