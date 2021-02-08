## usersテーブル

| Column     | Type   | Options  |
| ---------- | ------ | -------- |
| email      | string | NOT NULL |
| password   | string | NOT NULL |
| name       | string | NOT NULL |
| profile    | text   | NOT NULL |
| occupation | text   | NOT NULL |
| position   | text   | NOT NULL |

## commentsテーブル

| Column    | Type       | Options  |
| --------- | ---------- | -------- |
| text      | text       | NOT NULL |
| user      | references |          |
| prototype | references |          |

## prototypesテーブル

| Column  | Type          | Options  |
| ------- | ------------- | -------- |
| title   | string        | NOT NULL |
| catch   | text          | NOT NULL |
| concept | text          | NOT NULL |
| image   | ActiveStorage |          |
| user    | references    |　　　　　　|
