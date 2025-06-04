AutoShop – User and Vehicle Management System

Project Description

This project includes an ASP.NET Core 6 API and a React 18 frontend for managing users and vehicles. Data is stored in either SQL Server or SQLite, and the code follows Clean Code and Best Practices principles.

Technologies Used

Backend:

ASP.NET Core 6

Entity Framework Core

SQL Server / SQLite

Dependency Injection

Auto Migration (Database.Migrate)

Automatic Seed Data

Console Logging

Frontend:

React 18

Axios

React Router DOM

Bootstrap or CSS

Installation and Running

Prerequisites:

.NET 6 SDK

Node.js + NPM

SQL Server installed (or Docker)

Run Backend:

cd AutoShop.API
# Restore dependencies
dotnet restore
# Apply database migrations and start server
dotnet ef database update
dotnet run

Default URL: http://localhost:5041

Run Frontend:

cd auto-shop-frontend
npm install
npm run dev

Accessible at: http://localhost:5173

Backend Architecture

Controllers – Expose HTTP endpoints and forward requests to services

Services – Contain business logic and interact with the DbContext

Models – Entity Framework classes representing database tables

DTOs – API-facing data transfer objects without exposing internal models

DbContext – Manages database connection, migrations, and seed data



