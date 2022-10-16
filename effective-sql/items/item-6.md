## Item 6: Define FK to protect referential integrity
- why? referential integrity
- `post has many comments`
    - ensure no comment associates with non-existent post
    - `update cascade` -> update PK on post (1-side) will update FK on comments (m-side) 
    - `delete cascade` -> delete post will delete all associated comments