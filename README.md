# Very Slow Fibonacci Calculator

This respository is a basic level dockerized React Application which calculates the nth Fibonacci number
and stores the value in a PostgreSQL database and caches the values in a Redis Worker as a worker module
computes the values in the background.

## To Get Started

1. Clone the repository to your local machine and ensure you have Docker running on your machine. 

2. Navigate to the complex directory by running `cd complex`

3. To create the Docker images and build the application run `docker-compose up --build` or `docker compose up --build`


## To Stop The Application 

Run `docker-compose down` or `docker compose down`