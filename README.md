# テーブル設計

## usersテーブル

|Column   | Type   | Options     |
|-------- | ------ | ----------- |
| name    | string | null: false |
| email   | string | null: false |
| pasword | string | null: false |

## roomsテーブル
|Column   | Type   | Options     |
|-------- | ------ | ----------- |
| name    | string | null: false |

### Association

## room_users　テーブル

|Column   | Type   | Options     |
|-------- | ------ | ----------- |
| user    | reference | null: false, foreign_key: true |
| room    | reference | null: false, foreign_key: true |

### Association

## messages　テーブル

|  Column   | Type       | Options     |
| --------  | ------     | ----------- |
|  content  | string     | Options     |
| user      | references | null: false, foreign_key: true |
| room      | references | null: false, foreign_key: true |


### Association

- belongs_to :room
- belongs_to :user






# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
