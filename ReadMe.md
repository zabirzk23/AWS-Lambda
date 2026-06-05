# Experiment: AWS Lambda
## Author

### Name : Mohamed Zabir Khan A
### Register Number: 212224230162

## AIM

* To create an AWS Lambda function.
* To configure the Lambda function.
* To verify that the Lambda function works correctly.
* To understand the effect of IAM policies on service access.

---

## PROBLEM STATEMENT

AWS Lambda is a serverless computing service that allows users to run code without provisioning or managing servers. The objective of this experiment is to create a Lambda function, configure its settings, execute it, and observe how IAM permissions affect access to AWS resources.

---

## ALGORITHM

### Step 1:

Log in to the AWS Management Console.

### Step 2:

Navigate to **AWS Lambda** and select **Create Function**.

### Step 3:

Choose **Author from Scratch**, enter the function name, select the runtime (Python 3.x), and create a new execution role.

### Step 4:

Enter the Lambda function code and click **Deploy**.

### Step 5:

Create a test event, execute the function, and verify the output in the execution results and CloudWatch logs.

---

## COMMANDS

### Lambda Function Code (Python)

```python
def lambda_handler(event, context):
    return {
        'statusCode': 200,
        'body': 'Hello from AWS Lambda!'
    }
```

### Test Event JSON

```json
{
  "key1": "value1",
  "key2": "value2"
}
```

---

## OUTPUT

### AWS Lambda Function Created

**Function Name:** MyLambdaFunction

**Runtime:** Python 3.12

**Handler:** lambda_function.lambda_handler

**Status:** Active

---

### Lambda Function Code Screen

```python
def lambda_handler(event, context):
    return {
        'statusCode': 200,
        'body': 'Hello from AWS Lambda!'
    }
```

---

### Test Execution Result

```json
{
  "statusCode": 200,
  "body": "Hello from AWS Lambda!"
}
```

---

### CloudWatch Log Output

```text
START RequestId: xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
END RequestId: xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
REPORT RequestId: xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
Duration: 1.25 ms
Billed Duration: 2 ms
Memory Size: 128 MB
Max Memory Used: 65 MB
```

---

## OUTPUT SCREENSHOTS TO INCLUDE

<img width="1919" height="915" alt="image" src="https://github.com/user-attachments/assets/f35898bb-eace-42b1-81db-0995af228ab0" />

<img width="750" height="514" alt="image" src="https://github.com/user-attachments/assets/c68e6a78-3fe0-4493-b969-32ec4ac80c6c" />

<img width="1919" height="573" alt="image" src="https://github.com/user-attachments/assets/4dab12eb-b6e7-4983-91c0-7ce81b534d83" />


## RESULT

The AWS Lambda function was successfully created, configured, deployed, and tested. The function executed successfully and returned the expected output. IAM policies were examined to understand how permissions control access to AWS services. Thus, the objectives of creating and verifying an AWS Lambda function were achieved successfully.
