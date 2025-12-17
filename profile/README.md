# MoonTrade

MoonTrade is a multi-repository project implementing a zero-risk cryptocurrency
trading simulator with real-time market mechanics.

The project is split into multiple repositories to clearly separate
backend logic, client applications, and infrastructure concerns.

## Repositories

- **moontrade_server**  
  Backend service responsible for all trading logic, order matching,
  balance updates, and real-time data delivery.

- **MoonTrade**  
  Android client application built with Kotlin and Jetpack Compose.
  Focused on UI, user interaction, and real-time visualization.

- **moontrade_db**  
  Database schema, migrations, and persistence-related configuration
  (if separated from backend).

## External Resources

- **Product landing page (UI preview)**  
  https://qusterrr.github.io/mt-landing/

> The landing page is a visual and conceptual preview of the product.
> It is not part of the core project repositories and does not contain
> backend logic or trading functionality.

## Architectural Principles

- Backend is the single authority for all trading logic
- Database is the single source of truth
- Client applications contain no business rules
- Authentication is centralized and verified server-side
- Real-time updates are delivered via WebSockets

## Project Status

Active development.
