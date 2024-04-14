# AWS Identity and Access Management

## IAM

**IAM** is used to **manage permissions**.

## Users
An **user** is mapped to a **real world person**.  
Can belong to **multiple groups**, or no group at all.

## Groups
A **group** is a set of users.

## Policies

A **policy** is a **JSON** document describing **user or group permissions**

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow", // Or Deny
      "Action": "ec2:ModifyImageAttribute", // Action to allow / deny
      "Resource": "arn:aws:ec2:us-east-1::image/ami-*", // AWS service which the action is applied to
      "Condition": { // Optional
        "StringEquals": {
          "ec2:Attribute/Description": [
            "Production",
            "Development"
          ]
        }
      }
    }
  ]
}
```

## MFA: Multi Factor Authentication

Use a **real device that you own** to unlock your account, **should be used everywhere**.

## Access Keys

Used to access **AWS API**.

## AWS SDK

Wrapper around the AWS API, to use when **programming**. Requires an access key.

## AWS CLI

**CLI wrapper** around AWS API. Requires an access key.

## AWS CloudShell

An **online terminal** to access **AWS CLI**.

## IAM Roles

Permissions **but for AWS services**. If a service need to interact with another.

## IAM Security Tools

- **IAM Credentials Report**: Report all users credentials status
- **IAM Access Advisor**: Show the permissions granted to an user and the last access.

## IAM Access Analyzer

Monitor access to services. Recap resource policies for taking actions.

## Shared responsibility model

- **AWS: Infrastructure**, Configuration, Vulnerability analysis, Compliance Validation
- **User: Internal security**, policies, key rotation, permissions.
