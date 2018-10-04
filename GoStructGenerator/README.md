# Go Struct Generator
What this does?
This creates go lang structs for a mysql table, along with its db column name .

#How it works? 
Run following in the command line (at the location of this file) 


`go run go-struct-generator.go -u=root -p=12345 -d=test_db -t=contacts`

#Mandatory Parameters 
1. `u` ==> username 
2. `p` ==> password 
3. `d` ==> Db name 
4. `t` ==> table name

#Optional Parameters
1. `j` ==> If you also want to generate json tags. If you do not specify this flag, then json tags won't be generated. Permitted values are true and false.
Examples:
    1. `go run go-struct-generator.go -u=root -p=12345 -d=test_db -t=contacts`
        
        No json tags are generated.
    2. `go run go-struct-generator.go -u=root -p=12345 -d=test_db -t=contacts -j=false`
        
        No json tags are generated.
    3. `go run go-struct-generator.go -u=root -p=12345 -d=test_db -t=contacts -j=true`
        
        json tags are generated.



#Go Query Generator 
What this does?
Generates Select Query with all columns

#How it works? 
Run following in the command line (at the location of this file) 

go run go-query-generator.go -u=root -p=pass -d=database -t=table 

#Mandatory Parameters 
1. `u` ==> username 
2. `p` ==> password 
3. `d` ==> Db name 
4. `t` ==> table name