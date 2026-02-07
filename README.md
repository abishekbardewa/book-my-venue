# Book My Venue

## Overview
**Book My Venue** is a venue discovery and booking platform that allows users to search, reserve, and pay for event venues, while enabling venue owners to manage listings, availability, and bookings through a dedicated dashboard.  
The frontend focuses on **performance, reliability, and smooth booking experiences** across complex user flows.

---

## Core User Flows
- Venue discovery with location-based search, filters, and infinite scrolling  
- Detailed venue pages with availability calendars and media galleries  
- Secure booking flow with payment integration and status-tracked reservations  
- Offline-safe booking staging to prevent data loss during network failures  
- Owner dashboard for venue onboarding, listing management, and booking approvals  

---

## Key Engineering Decisions
- **State management**: Used Redux Toolkit to manage complex booking, authentication, and UI state across multi-step flows while keeping updates predictable and debuggable.  
- **Reliability & offline handling**: Implemented IndexedDB-based staging for booking requests to reduce dropped transactions during intermittent connectivity.  
- **Performance optimization**: Applied code splitting, lazy loading, and memoization to keep initial load times low and maintain responsive interactions on large result sets.  
- **Scalable UI architecture**: Designed reusable, accessible UI components and role-based layouts to support both consumer and owner workflows.  
- **API integration**: Centralized API handling with interceptors for authentication, retries, and consistent error feedback across the app.

---

## Tech Stack
- React 18, TypeScript  
- Redux Toolkit  
- React Router  
- IndexedDB (offline staging)  
- REST APIs  
