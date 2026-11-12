# ZedPay_Database_project
A database for a fictional fintech Banking app called ZedPay that expects to have 200,000 daily users and 50,000 transactions a day.

---

## Database Overview
This database  stores, organizes, and processes financial records, user identities, and real-time transactions for the ZedPay mobile Banking app.

---

## Table Documentation

| Table Name | Description |
|-----------|-----------|
| Users | Stores registered cutomer accounts|
|Merchants| Stores mercant deatiles |
| Transactions | Records user transactions |
| Agents | Stores agent detailes |
| Wallets | Stores cutomer wallet balances |
| Contact_details | Stores user | contact deatils |
|Location| Stores user locations 

---

### Users Table Structure 
| Field name | Type | isUnique | isNull | Example values |
|------------|------|----------|------------|----------------|
| user_id | INT | True | False| 0001,0002,
| first_name | VARCHAR | False | False | Ben, Emmanuel|
| last_name | VARCHAR | False | False | Mwape, Nachimata|
| adress_id | INT | False | False | 0002, 0024|
| user_tpin | INT | True | False | 2022005678, 7665989012 |
| user_type | VARCHAR | False | False | Merchant, Domestic, Agent |
|activity_status| VARCHAR | False | False | Active , Inactive |

### Merchant Table Structure
| Field name | Type | isUnique | isNull | Example values |
|------------|------|----------|------------|----------------|
| merchant_id | INT| TRUE |False| 1287,1290|
| user_id | INT | False | True | 54767, 76987|
| business_name | VARCHAR | False | False | FrontMark Trading, ShopRight|
| business_tpin | INT | True | False | 3276549865, 698438765 |  

### Transaction Table Structure

| Field name | Type | isUnique | isNull | Example values |
|------------|------|----------|------------|----------------|
| transation_id| INT | True | False | 8982, 2343|
| currency | VARCHAR | False | False | USD, ZMW |
| from_account_id | INT | False | False | 9023, 3245 |
| to_account_id | INT | False | False | 9023, 3245 | 
| amount | DECIMAL | False | False | 2000, 10000 |
| transaction_status | VARCHAR | False | False | Pending, Failed, completed |
| created_at | DATETIME | False | False | 2026-11-12 14:30:00.000 |


