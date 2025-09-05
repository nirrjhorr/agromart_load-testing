JMeter Performance Testing – AgroMart E-commerce Project
This repository showcases performance testing for the AgroMart e-commerce platform using Apache JMeter. AgroMart is a MERN stack-based website designed for buying and selling agricultural products.
Project Description
AgroMart is an online marketplace built with MongoDB, Express.js, React.js, and Node.js. Key features include:

Browsing and purchasing agricultural products
Managing shopping carts
User account creation and management
Order placement and tracking

This project tests the website's performance under varying user loads (100, 200, and 300 threads) to evaluate scalability and response times.
Project Structure
jmeter_project/
├── tests/       # JMeter test plan files (.jmx)
├── results/     # JMeter results files (.jtl)
├── reports/     # HTML dashboard reports
└── images/      # Screenshots of reports
    ├── T100.png
    ├── T200.png
    └── T300.png

Sample HTML Reports
T100 Threads

T200 Threads

T300 Threads


Running the Tests

Install Apache JMeter.
Execute test plans in non-GUI mode:

jmeter -n -t tests/agromart_t100.jmx -l results/results_t100.jtl
jmeter -n -t tests/agromart_t200.jmx -l results/results_t200.jtl
jmeter -n -t tests/agromart_t300.jmx -l results/results_t300.jtl


Generate HTML reports:

jmeter -g results/results_t100.jtl -o reports/html_report_t100
jmeter -g results/results_t200.jtl -o reports/html_report_t200
jmeter -g results/results_t300.jtl -o reports/html_report_t300

Skills Demonstrated

Creating and executing JMeter test plans with thread groups and listeners
Conducting load tests for 100, 200, and 300 concurrent users
Generating and analyzing HTML dashboard reports
Performance testing a MERN stack e-commerce application
