# WebLogInsights

---

# Log Analysis Tool

## Objective
This Python-based project processes log files to extract, analyze, and report key information. It is designed to demonstrate file handling, string manipulation, and data analysis skills relevant to cybersecurity and system monitoring tasks.

---

## Features

 # 1.Count Requests per IP Address  
   - Analyzes log files to identify the number of requests made by each IP address.
   - Displays results sorted by the highest request count.

 # 2.Identify the Most Frequently Accessed Endpoint  
   - Extracts and identifies the most accessed resource (e.g., URLs or endpoints) from the log file.

 # 3.Detect Suspicious Activity  
   - Identifies potential brute force login attempts based on repeated failed login entries.
   - Flags IP addresses with excessive failed login attempts.
# 4.Output Results  
   - Displays results in a terminal-friendly format with clear headings.
   - Saves results to a single CSV file named `log_analysis_results.csv` for easy sharing and review.

## Example Outputs

### Terminal Output
```plaintext
=== Requests per IP ===
IP Address       Request Count
192.168.1.1      234
203.0.113.5      187
10.0.0.2         92

=== Most Accessed Endpoint ===
Endpoint          Access Count
/home             403
/login            298
/dashboard        122

=== Suspicious Activity ===
IP Address       Failed Login Attempts
192.168.1.100    56
203.0.113.34     12
```

### CSV Structure
The `log_analysis_results.csv` file contains three sheets:
1. ## Requests per IP
   - `IP Address`, `Request Count`
2. ## Most Accessed Endpoint
   - `Endpoint`, `Access Count`
3. ## Suspicious Activity
   - `IP Address`, `Failed Login Count`

---

## **Configuration**
- # Suspicious Activity Threshold
-  You can modify the threshold for failed login attempts (default is 10) by changing the variable `FAILED_LOGIN_THRESHOLD` in `log_analysis.py`.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details

---

## Contact
Created by [syedzameer](https://github.com/syedzameer18)  
For questions or contributions, feel free to reach out!

---

Let me know if you'd like help customizing this further!
