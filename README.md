# eCommerce Microservices (.NET)

A .NET microservices-based e-commerce backend, split into independent services for products, users, and orders — built while learning distributed systems and microservice architecture patterns.

> Note: this project follows a well-known .NET microservices course/tutorial structure. I'm not hiding that — I'm being upfront about it here, and this README exists to make clear what I built, understood, and extended beyond the base tutorial.

## What this covers

- **ProductsService** 
- **UsersService** 
- **OrdersService**


## Architecture

```
┌────────────────┐     ┌────────────────┐     ┌────────────────┐
│ ProductsService│     │  UsersService  │     │  OrdersService │
└───────┬────────┘     └───────┬────────┘     └───────┬────────┘
        │                      │                       │
        └──────────────────────┴───────────────────────┘
                        [
```

## Tech stack

- .NET 8 / C#
- Database used — PostgreSQL
- Docker

## Running locally

```bash
git clone https://github.com/agrahariaman238-work/eCommerceSolution.ProductsService.git
cd eCommerceSolution.ProductsService
dotnet restore
dotnet run
```
Repeat for each service, and add any docker-compose command if you have one that runs all three together.

## What I'd improve next
add an API gateway, add integration tests across services, add centralized logging.
