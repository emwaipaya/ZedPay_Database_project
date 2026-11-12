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
|activity_status| VARCHAR | False | False | Active , Inactive |\
| contact_id | INT | False | False | 9890, 325476|

### Merchant Table Structure
| Field name | Type | isUnique | isNull | Example values |
|------------|------|----------|------------|----------------|
| merchant_id | INT| TRUE |False| 1287,1290|
| user_id | INT | False | True | 54767, 76987|
| business_name | VARCHAR | False | False | FrontMark Trading, ShopRight|
| business_tpin | INT | True | False | 3276549865, 698438765 |
| contact_id | INT | False | False | 9890, 325476|

### Transaction Table Structure
| Field name | Type | isUnique | isNull | Example values |
|------------|------|----------|------------|----------------|
| transation_id| INT | True | False | 8982, 2343|
| currency | VARCHAR | False | False | USD, ZMW |
| from_id | INT | False | False | 9023, 3245 |
| to_id | INT | False | False | 9023, 3245 |
| trans_description | VARCHAR | False | True | Food, rent |
| amount | DECIMAL | False | False | 2000, 10000 |
| transaction_status | VARCHAR | False | False | Pending, Failed, completed |
| created_at | DATETIME | False | False | 2026-11-12 14:30:00.000 |

### Agents Table Structure
| Field name | Type | isUnique | isNull | Example values |
|------------|------|----------|------------|----------------|
| agent_id | INT | True | False | 9876, 1254 |
| user_id | INT | False | True | 8723, 2439|
|location_id| INT | False | False | 9823, 2345|
| contact_id | INT | False | False | 9890, 325476|

### Wallets Table Structure
| Field name | Type | isUnique | isNull | Example values |
|------------|------|----------|------------|----------------|
| wallet_id | INT | True | False | 9034, 5465 |
| user_id | INT | False | False | 7632, 23643 |
| balance | DECIMAL | False | False | 7.00, 10,100.50|
| last_update | DATETIME | False | False | 2026-11-12 14:30:00.000 |
| created_at | DATETIME | False | False | 2026-11-12 14:30:00.000 |

### Contact_details Table Structure
| Field name | Type | isUnique | isNull | Example values |
|------------|------|----------|------------|----------------|
| contact_id | INT | True | False | 12034, 3409 |
| number | VARCHAR | True | False | 0960097894, 0779540223|
| email | VARCHAR | True | False | example@provider |

### Location Table Structure
| Field name | Type | isUnique | isNull | Example values |
|------------|------|----------|------------|----------------|
| location_id | INT | True | False | 903287, 2349854|
| province | VARCHAR | False | False | Copperbelt, Lusaka |
| city | VARCHAR | False | False | Kitwe, Kasama|
| region | VARCHAR | False |True | Chachacha, matero|
| home_adress | VARCHAR | False | False |(cc3, lunda), (388, first Street) 





|-|-|-|-|-|