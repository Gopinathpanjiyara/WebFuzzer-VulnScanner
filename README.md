# Web Vulnerability Fuzzer with Crawl and Attack Simulation

## Description:

The **Web Vulnerability Fuzzer with Crawl and Attack Simulation** is an automated security testing tool designed to identify and report vulnerabilities in web applications. It integrates web crawling, security attack simulations, and a detailed vulnerability report generation system to ensure comprehensive security audits.

This project performs the following operations:
1. **Web Crawling**: Automatically crawls the provided web application URLs to discover endpoints, forms, and other resources.
2. **Attack Simulation**: Performs common attack simulations like XSS (Cross-Site Scripting), SQL Injection, and Command Injection on the discovered endpoints.
3. **Fuzzing**: Simulates various attack vectors to uncover vulnerabilities and analyze web app behavior under malicious input.
4. **Real-Time Reporting**: Generates detailed vulnerability reports categorizing issues by severity (High, Medium, Low) for each URL scanned.

With this tool, security professionals and web developers can test their applications for known vulnerabilities and ensure they are prepared against common web attacks.

---

## Features:

- **Automated Crawling**: Automatically crawls through the target URLs to detect all accessible endpoints.
- **Security Attack Simulation**: Simulates various attack types like XSS, SQL Injection, and Command Injection.
- **Fuzz Testing**: Automatically fuzzes the web application to uncover hidden vulnerabilities.
- **Detailed Reporting**: Provides real-time reporting of detected vulnerabilities, categorized by severity.
- **Customizable Attack Options**: Allows the user to select specific attacks to perform or choose all attacks at once.
- **Session Management**: Automatically creates and manages a new session in ZAP (OWASP Zed Attack Proxy) to track and manage scans.

---

## Prerequisites:

Before running the tool, make sure the following are installed and properly configured:
- **OWASP ZAP (Zed Attack Proxy)**: A security testing tool used to perform the attack simulations.
- **Python 3.x**: Required for running the fuzzer and all associated scripts.
- **Python Libraries**:
    - `requests`: For handling HTTP requests.
    - `termcolor`: For colorful terminal output.
    - `datetime`: For time tracking.
    - `crawler`, `attack`, `report_generator`, `connection`: Custom modules for crawling, attacking, and reporting.
  
You can install the required Python libraries using:

```bash
pip install requests termcolor
