
```markdown
# AgroMart Load Testing with JMeter

This repository contains performance testing setup and results for the **AgroMart** e-commerce platform using **Apache JMeter**. AgroMart is a MERN stack-based website for buying and selling agricultural products.

## Project Description

AgroMart is an online marketplace built with MongoDB, Express.js, React.js, and Node.js. Key features include:
- Browsing and purchasing agricultural products
- Managing shopping carts
- User account creation and management
- Order placement and tracking

This project tests AgroMart's performance under 100, 200, and 300 concurrent users to evaluate scalability and response times.

## Project Structure

```
gromart_load-testing/
├── tests/       # JMeter test plan files (.jmx)
├── results/     # JMeter results files (.jtl)
├── reports/     # HTML dashboard reports
└── images/      # Screenshots of test reports
    ├── T100.png
    ├── T200.png
    └── T300.png
```

## Sample Test Report Screenshots

### 100 Threads
![100 Threads](https://github.com/nirrjhorr/agromart_load-testing/blob/ee2aa17e64932bce24d648f6efd0b3db4ff11054/images/T100.png)

### 200 Threads
![200 Threads](https://github.com/nirrjhorr/agromart_load-testing/blob/ee2aa17e64932bce24d648f6efd0b3db4ff11054/images/T200.png)

### 300 Threads
![300 Threads](https://github.com/nirrjhorr/agromart_load-testing/blob/ee2aa17e64932bce24d648f6efd0b3db4ff11054/images/T300.png))

## Running the Tests

1. Install [Apache JMeter](https://jmeter.apache.org/).
2. Run test plans in non-GUI mode:

```bash
jmeter -n -t tests/agromart_t100.jmx -l results/results_t100.jtl
jmeter -n -t tests/agromart_t200.jmx -l results/results_t200.jtl
jmeter -n -t tests/agromart_t300.jmx -l results/results_t300.jtl
```

3. Generate HTML reports:

```bash
jmeter -g results/results_t100.jtl -o reports/html_report_t100
jmeter -g results/results_t200.jtl -o reports/html_report_t200
jmeter -g results/results_t300.jtl -o reports/html_report_t300
```

## Skills Demonstrated

- Designing JMeter test plans with thread groups, samplers, and listeners
- Executing load tests for 100, 200, and 300 concurrent users
- Generating and analyzing HTML dashboard reports
- Performance testing a MERN stack e-commerce application

## Setup for GitHub

1. Save this file as `README.md` in the root of your `gromart_load-testing` repository.
2. Ensure the `images/` folder contains `T100.png`, `T200.png`, and `T300.png`.
3. Commit and push to GitHub.
```

