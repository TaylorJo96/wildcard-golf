# Wildcard Golf ⛳

A full-stack golf league app where players create leagues, invite friends,
schedule matches with tee times, record scores and track standings.

Built in 2 weeks as the final capstone at Tech Elevator (2022) by a team of 4,
working with a product owner and presented at a public open house.

**Tech:** Vue 2 · Vuex · Vue Router · Axios · ASP.NET Core 3.1 Web API · C# ·
SQL Server · JWT auth · Google Maps Embed API · OpenWeather API

## Features
- Register / log in with JWT-secured routes
- Create leagues at a course and invite players (accept / decline invites)
- Find courses with an embedded Google Maps search; view local weather per course
- Schedule matches and assign tee times
- Record scores; view league leaderboards and personal score history

## My role
I worked across the full stack with my team. I built much of the Vue front end
(views, components, routing, the Vuex store and the Axios service layer) and
contributed to the ASP.NET Core API, data access layer and SQL Server database.

## Reflection
Wildcard Golf was my first full-stack application built from the ground up. In
two weeks, our team took it from a product owner's requirements to a working app
we presented at Tech Elevator's public open house. Along the way I learned to
plan and divide work across a team, design a relational database, secure an API
with JWT authentication, integrate third-party APIs, and connect a Vue front end
to a .NET back end.

## Running locally
Requires SQL Server Express, the .NET Core 3.1 SDK and Node.js.

1. Run [`dotnet/database/capstone.sql`](dotnet/database/capstone.sql) against SQL Server Express to create the `final_capstone` database
2. Start the API: `cd dotnet/Capstone && dotnet run`
3. Start the front end: `cd vue && npm install && npm run serve`
4. Log in with the default account `user` / `password`, or register a new one

## Project structure
```
dotnet/   ASP.NET Core Web API: controllers, DAOs, models, JWT security, SQL scripts
vue/      Vue 2 front end: views, components, router, Vuex store, API services
```

The [`dotnet/README.md`](dotnet/README.md) and [`vue/README.md`](vue/README.md)
files are the original Tech Elevator starter-project guides this app was built from.
