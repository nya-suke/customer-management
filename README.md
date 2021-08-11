# テーブル設計

## customerテーブル

| Column               | Type        | Options                                     |
|:---------------------|------------:|:-------------------------------------------:|
| date             | date      | null: false                                 |
| last_name                | string      | null: false, unique: true                   |
| first_name   | string      | null: false                                 |
| last_name_kana            | string      | null: false                                 |
| first_name_kana           | string      | null: false                                 |
| gender_id       | integer      | null: false                                 |
| birth_date      | date     | null: false                                 |
| postal_code     | string      | null: false                                 |
| prefecture_id     | integer      | null: false                                 |
| city      | string      | null: false                                 |
| address     | string      | null: false                                 |
| phone_number      | string      |                                 |
| email     | string      |                                 |
| companion     | string      |                                |
| introducer     | string      |                                  |
| notice      | string      |                           |

## Association
 has_many: records



 ## recordsテーブル

| Column                | Type        | Options                         |
|:---------------------:|------------:|:-------------------------------:|
| date              | date      | null: false                     |
| manager          | string       | null: false                     |
| purpose          | string     | null: false                     |
| response            | string     | null: false                     |
| result       | string     | null: false                     |
| others        | string     |                      |
| customer | reference     | null: false, foreign_key: true                     |




## Association
 belongs_to: customer
 

