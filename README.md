# データベース設計

## users テーブル
| カラム名             | データ型      | 制約                          |
|----------------------|---------------|-------------------------------|
| email               | STRING        | NOT NULL, UNIQUE             |
| encrypted_password  | STRING        | NOT NULL                     |
| name                | STRING        | NOT NULL                      |
| role                | STRING        | DEFAULT: "fan", NOT NULL     |
| confirmation_sent_at| DATETIME      |                               |