**1. Find the 99th line of a file using only `tail` and `head` commands:**

To find the 99th line of a file, you can use the following command:

```bash
head -n 99 <file_name> | tail -n 1
```

**Explanation:**
- `head -n 99`: Displays the first 99 lines of the file.
- `tail -n 1`: Extracts the last line (the 99th line) from the output of the `head` command.

---

**2. Confirm how long a server has been running:**

To check how long a server has been running, you can use the `uptime` command:

```bash
uptime
```

**Output Example:**
```
 10:25:43 up 3 days,  4:12,  2 users,  load average: 0.01, 0.05, 0.08
```
- `up 3 days, 4:12`: Indicates the server has been running for 3 days and 4 hours, 12 minutes.

---

**3. Python program to count character occurrences in a string:**

```python
from collections import Counter

# Input string
input_string = "hello world"

# Count character occurrences
character_count = Counter(input_string)

# Display results
for char, count in character_count.items():
    print(f"'{char}' occurs {count} times")
```

**Output Example:**
```
'h' occurs 1 times
'e' occurs 1 times
'l' occurs 3 times
'o' occurs 2 times
' ' occurs 1 times
'w' occurs 1 times
'r' occurs 1 times
'd' occurs 1 times
```

---

**4. Container Life Cycle:**

A container’s life cycle involves the following states:

1. **Created:**
   - The container is created using an image but has not started yet.
   - Command: `docker create <image>`

2. **Running:**
   - The container is actively running a process.
   - Command: `docker start <container>`

3. **Paused:**
   - The container’s processes are temporarily stopped.
   - Command: `docker pause <container>`

4. **Stopped:**
   - The container is no longer running, but its data and configuration are preserved.
   - Command: `docker stop <container>`

5. **Removed:**
   - The container is deleted from the system.
   - Command: `docker rm <container>`

---

**5. What is EC2 in AWS, and how is it useful?**

**Amazon Elastic Compute Cloud (EC2):**
- EC2 is a web service that provides resizable compute capacity in the cloud.
- It allows users to launch virtual servers (instances) to run applications.

**Features and Use Cases:**
1. **Scalable Computing:** Scale up or down based on demand.
2. **Customizable Instances:** Choose instance types with specific vCPU, memory, and storage configurations.
3. **Elasticity:** Automatically adjust capacity with Auto Scaling.
4. **Variety of Pricing Models:** Options include On-Demand, Reserved, and Spot instances.
5. **Security:** Provides robust security with IAM roles, security groups, and key pairs.
6. **Use Cases:**
   - Hosting web applications.
   - Running batch jobs.
   - Big data analytics.
   - Development and testing environments.

---

**6. How AWS Lambda Works and Its Use Cases:**

**AWS Lambda:**
- AWS Lambda is a serverless compute service that runs code in response to events.
- It automatically manages the compute infrastructure required to run the code.

**How It Works:**
1. **Event Source:** An event triggers the Lambda function (e.g., an S3 upload, API Gateway request).
2. **Function Execution:** Lambda runs the code in a managed environment.
3. **Automatic Scaling:** Lambda automatically scales based on the number of requests.
4. **Pay-Per-Use:** You are charged based on the number of requests and the execution time.

**Use Cases:**
1. **Data Processing:** Process files uploaded to S3 or streaming data from Kinesis.
2. **Backend for APIs:** Serve as the backend for web and mobile applications via API Gateway.
3. **Automation:** Automate AWS resource management or perform scheduled tasks.
4. **IoT Applications:** Handle events from IoT devices.
5. **Real-Time Notifications:** Send alerts or notifications based on events.

---

**7. What is AWS CloudTrail?**

**AWS CloudTrail:**
- AWS CloudTrail is a service that records AWS account activity and API calls.
- It provides visibility into user activity by recording actions taken through the AWS Management Console, CLI, SDKs, and other AWS services.

**Features and Use Cases:**
1. **Logging and Monitoring:** Logs every API call made in your AWS account.
2. **Security Analysis:** Detect unauthorized or unusual activity.
3. **Compliance:** Helps meet compliance requirements by maintaining an auditable trail.
4. **Troubleshooting:** Identify the root cause of operational issues by reviewing logs.
5. **Forensics:** Track resource changes for security forensics.

**Example Use Case:**
- Identify who terminated an EC2 instance in your account by reviewing the CloudTrail logs.

---

