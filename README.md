# AWS IAM Security Implementation Project

## Project Overview
This project demonstrates how AWS Identity and Access Management (IAM) is implemented using best security practices such as least privilege access, Multi-Factor Authentication (MFA), and role-based access control.

## Project Objectives
- Secure AWS root account using MFA
- Create IAM users and groups
- Apply least privilege permissions using policies
- Enable MFA for IAM users
- Implement IAM roles for EC2 to access S3 securely
- Test permissions using different IAM users

## AWS Services Used
- AWS IAM
- Amazon EC2
- Amazon S3
- IAM Roles

## IAM Users
- AdminUser
- DevUser1
- DevUser2
- InternUser
- AuditorUser

## IAM Groups
- Admins – AdministratorAccess
- Developers – Custom EC2 policy
- Interns – Restricted access
- Auditors – Read-only access

## Security Features
- Root MFA enabled
- Strong password policy
- MFA for Admin and Developer users
- Least privilege principle

## IAM Role (EC2 → S3)
An IAM role named EC2S3Role was attached to an EC2 instance to allow access to S3 without using access keys.

### Test Command
aws s3 ls
## OutPut
ec2-static-media-001
## Permission Testing
Developers can start/stop EC2
Developers cannot terminate EC2
Interns have restricted access
## Outcome
Successfully implemented secure IAM architecture using AWS best practices.

