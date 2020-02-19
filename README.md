# DB設計

## usersテーブル

|Column|Type|Options|
|------|----|-------|
|name|string|null: false, add_index: true|
|email|string|null: false, unique: true|

### Association
- has_many :groups_users
- has_many :groups, through: groups_users
- has_many :messages

