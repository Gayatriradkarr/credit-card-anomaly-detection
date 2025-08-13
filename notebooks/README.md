# Credit Card Fraud Detection Using Behavioral Rules & Statistical Profiling

## Step 1: Load Data
import pandas as pd
import numpy as np
df = pd.read_csv('data/transactions.csv')

## Step 2: EDA
df['hour'] = pd.to_datetime(df['timestamp']).dt.hour
df['amount'].hist(bins=50)

## Step 3: Rule-Based Detection
df['high_amount_flag'] = df['amount'] > df['amount'].quantile(0.99)
df['off_hour_flag'] = df['hour'].between(2, 4)

## Step 4: Z-Score Profiling
df['z_score'] = (df['amount'] - df['amount'].mean()) / df['amount'].std()
df['z_flag'] = df['z_score'].abs() > 3

## Step 5: Export Flagged Transactions
df[df[['high_amount_flag', 'off_hour_flag', 'z_flag']].any(axis=1)].to_csv('flagged_transactions.csv', index=False)

