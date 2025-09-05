
```markdown
# JMeter Performance Testing – AgroMart E-commerce Project

This repository demonstrates my **Apache JMeter** skills for performance testing. The tests were performed on **[AgroMart](https://agromart.onrender.com/)**, a **MERN stack-based e-commerce website** for the agriculture business.

---

## Website Tested

AgroMart is an online platform for buying and selling agricultural products, built using **MongoDB, Express.js, React.js, and Node.js (MERN stack)**. Users can:

- Browse and purchase products
- Manage their shopping cart
- Create and manage accounts
- Place and track orders

---

## Project Structure

```

jmeter\_project/
├─ tests/       # JMeter test plan files (.jmx)
├─ results/     # JMeter results files (.jtl)
├─ reports/     # HTML dashboard reports
└─ images/      # Screenshots of reports
├─ T100.png
├─ T200.png
└─ T300.png

````

---

## Sample HTML Reports

### T100 Threads
![T100 Report](images/T100.png)

### T200 Threads
![T200 Report](images/T200.png)

### T300 Threads
![T300 Report](images/T300.png)

> Make sure the images are in the `images/` folder with the exact filenames above.

---

## Running the Tests

1. Install [Apache JMeter](https://jmeter.apache.org/)  
2. Run test plans in **non-GUI mode**:

```bash
jmeter -n -t agromart_t100.jmx -l ../results/results_t100.jtl
jmeter -n -t agromart_t200.jmx -l ../results/results_t200.jtl
jmeter -n -t agromart_t300.jmx -l ../results/results_t300.jtl
````

3. Generate HTML reports:

```bash
jmeter -g ../results/results_t100.jtl -o ../reports/html_report_t100
jmeter -g ../results/results_t200.jtl -o ../reports/html_report_t200
jmeter -g ../results/results_t300.jtl -o ../reports/html_report_t300
```

---

## Skills Demonstrated

* Apache JMeter: test planning, thread groups, listeners
* Load testing multiple scenarios (100, 200, 300 users)
* Generating and analyzing HTML dashboard reports
* Performance testing a MERN stack-based e-commerce website

```


