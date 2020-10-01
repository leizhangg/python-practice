Credit Assist v1.1

Our bank needs a tool that will help us in determining credit worthiness of loan applicants. We will enter the following information to Credit Assist program:

- Monthly Income (income)

- Total Debt (debt)

- Monthly minimum payments for the debt (minPay)

If total debt is more than 6 months monthly income of the applicant (income*6), we cannot grant any loan. Inform user that no loan can be granted. 

Otherwise, you subtract the minimum monthly debt payment from monthly income. We can allow up to 30% of that amount as loan. 

credit = (income - minPay) * 0.3

Let user know that the applicant can be approved for upto this (credit) amount. 



#!/usr/bin/env python3
# -*- coding: utf-8 -*-
"""
Created on Sat Sep 5 01:13:31 2020
@author: ZL
"""
income = int( input("Enter your income : "))
debt = int(input("Enter your debt: "))
miniPay = int(input ("Enter your minimum payments for the debt: "))
credit = (income - miniPay) * 0.3
if debt > income * 6:
print("We cannot grant any loan")
else:
print(" We can grant up to ", credit)
