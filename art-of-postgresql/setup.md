# Setup

- docker cp files/appdev.dump sqlfluency-pg:/mydata
- pg_restore -U postgres -d postgres -x mydata