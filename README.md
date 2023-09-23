# the-knight-shop

#Database
# Script create migrations file
migrate create -ext sql {db_name} -seq 

# Script Migration DB
migrate -source file://{path} -database 'postgres://{username}:{password}@{host}:{port}/{db_name}?sslmode=disable' -verbose up


