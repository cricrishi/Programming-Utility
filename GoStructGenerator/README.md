# Go Struct Generator
What this does?
This creates go lang structs for a mysql table, along with its db column name .

#How it works? Run following in the command line (at the location of this file) go run struct-generator.go -u=root -p=12345 -d=test_db -t=contacts

This command takes 4 paramters: 1. u ==> username 2. p ==> password 3. d ==> Db name 4. t ==> table name

#Go Query Generator 
Generates Select Query with all columns

go run go-query-generator.go -u=root -p=pass -d=database -t=table 
