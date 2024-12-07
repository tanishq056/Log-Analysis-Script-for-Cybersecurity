# Log Analysis Script for Cybersecurity
## 🚀 Overview
This Python script analyzes server log files to extract key insights such as traffic patterns, suspicious login attempts, and the most accessed endpoints. It helps identify potential brute-force attacks and provides a clear summary of network activity.

## 🔑 Key Features:

1. Count Requests per IP Address: Identify traffic sources by counting requests made by each IP address.

2. Find the Most Frequently Accessed Endpoint: Highlight the most popular resource or URL in the log file.

3. Detect Suspicious Activity: Detect IPs with excessive failed login attempts (default threshold: 2 attempts).

4. Export Results: Save the analyzed data to a CSV file for further use or reporting.

## 📋 Requirements
- Python 3.x

- Built-in libraries:

- re (Regular Expressions)

- collections.defaultdict and collections.Counter

csv

## 📂 Installation
1.Clone the repository:

  git clone https://github.com/tanishq056/Log-Analysis-Script-for-Cybersecurity

  cd log-analysis-script

2.Ensure Python 3.x is installed. Download it from python.org if needed.

3.Place your log file (e.g., sample.log) in the project directory.


## 📁 Code Structure

- parse_log(file_path): Parses the log file and extracts:

- IP addresses

- Accessed endpoints

- Failed login attempts

- count_requests_per_ip(ip_addresses): Counts and sorts requests by IP.

- find_most_accessed_endpoint(endpoints): Finds the most accessed URL or resource.

- display_suspicious_activity(failed_logins, threshold=2): Displays suspicious IP addresses with failed login attempts above the specified threshold.

- save_to_csv(ip_data, endpoint_data, suspicious_data, output_file): Saves results into a CSV file.

## 📊 Sample Output

Terminal                       Output

IP Address          -           Request Count

192.168.1.1         -           45

192.168.1.2         -           30

Most Frequently Accessed Endpoint:

/login (Accessed 60 times)

Suspicious Activity Detected:

IP Address           -          Failed Login Attempts

192.168.1.5          -          5

192.168.1.10         -          3


----------------------------------------------------------------------------------------------------------------------

Google Collab Link For File :- https://colab.research.google.com/drive/1l6d7KKUb_1WxYUgTeZwqK4_1Gfm-fjrg?usp=drive_link

Instruction :- 
  
1.Upload the sample.log file in the "Files"  section in Google Collab

2.Run the code and check the saved CSV file in the "Files" section in Google collab

