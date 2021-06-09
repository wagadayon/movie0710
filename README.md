## users table

| Column             | Type                | Options                 |
|--------------------|---------------------|-------------------------|
| email              | string              | null: false             |
| password           | string              | null: false             |
| name               | string              | null: false             |
| profile            | text                | null: false             |
| occupation         | text                | null: false             |
| position           | text                | null: false             |


* has_many :comments



## comments table

| Column      | Type       | Options           |
|-------------|------------|-------------------|
| text        | text       | null: false       |
| user        | references | foreign_key: true |

### Association


- belongs_to :user
