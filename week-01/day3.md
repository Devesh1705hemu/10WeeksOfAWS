# 🔐 AWS Labs: Account Security & Billing

## Lab 1 - Secure Root User

### 🎯 Objective

Secure the AWS Root User by enabling **Multi-Factor Authentication (MFA)** and avoiding the Root User for daily AWS tasks.

### 🛠️ Steps

1. Create or log in to your AWS account.
2. Search for `IAM` in the AWS Console.
3. Open the security recommendations or MFA settings.
4. Enable MFA on the Root User.
5. Stop using the Root User for daily work.
6. Create an IAM admin user only if needed for regular work.

### 📦 Deliverables

#### 📸 Screenshot of Root MFA Enabled

<img width="1020" height="800" alt="Screenshot 2026-08-17 005826(1)" src="https://github.com/user-attachments/assets/5af97cba-1fea-4f49-9507-5125fd57568c" />

<!-- CONTRIBUTING -->
```text
![Root MFA Enabled](root-mfa-enabled.png)

**Result:** MFA has been successfully enabled on the AWS Root User. This adds an extra layer of security to the AWS account.

### 📝 Why Root User should not be used daily

The Root User has full access to the AWS account. Using it daily can increase the risk of accidentally changing or deleting resources.

For daily work, it is safer to use an IAM user or role with only the required permissions.




