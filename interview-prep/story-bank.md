# STAR Story Bank â€” Bijith P N

This file stores STAR+R (Situation, Task, Action, Result + Reflection) stories for interview preparation, mapped to your Flutter experience.

## Technical Leadership & Architecture

### Re-architecting Legacy Codebase (Intersmart Solutions)
- **Situation:** Inherited a legacy Flutter project with high technical debt, spaghetti code, and frequent production crashes.
- **Task:** Improve stability, maintainability, and implement a scalable state management pattern.
- **Action:** Conducted a comprehensive code audit. Refactored the app layer by layer into Clean Architecture. Replaced inconsistent state logic with **Bloc** for complex modules and **GetX** for simpler ones. Implemented unit tests for critical business logic.
- **Result:** Reduced critical production bugs by 60% and halved the time required to onboard new features.
- **Reflection:** Solidified the importance of decoupled architecture for long-term project health.

### SQL Connection Plugin (Open Source)
- **Situation:** Needed a way for a Flutter app to talk directly to a legacy MS SQL Server without a middle-tier REST API for a specific enterprise client.
- **Task:** Create a reusable native bridge for direct SQL connectivity.
- **Action:** Developed a custom Flutter plugin using **MethodChannels** to communicate with native Android (Java/Kotlin). Handled database connection pooling and secure credential management on the native side while exposing a clean Dart API.
- **Result:** Published as an open-source package. Enabled the client to leverage their existing infrastructure without costly API refactoring.
- **Reflection:** Deepened my understanding of Flutter's platform-native interoperability.

## Real-time & Product Impact

### Real-time Football App (Shabab Al Ahli)
- **Situation:** Building the official app for a major football club requiring zero-latency match updates for thousands of concurrent fans.
- **Task:** Integrate real-time stats and ticketing.
- **Action:** Optimized WebSocket connections for live scores. Integrated the Platinumlist SDK for ticketing and used WordPress REST APIs for dynamic news feeds.
- **Result:** Successfully supported thousands of fans during live matches with real-time push notifications and smooth ticket booking.
- **Reflection:** High-traffic applications require rigorous testing of data synchronization and media-rich UI performance.

### Offline-First Sales Management (SalesSpark)
- **Situation:** Field sales teams often worked in areas with poor or no network connectivity, losing data during sync.
- **Task:** Implement an offline-first architecture.
- **Action:** Used **Hive** and **SQLite** for local caching. Built a robust synchronization engine that queues outgoing data and resolves conflicts once a connection is re-established.
- **Result:** Eliminated data loss reports from field teams and improved user satisfaction by 80%.
- **Reflection:** Designing for the "worst-case" connectivity scenario leads to much more resilient products.
