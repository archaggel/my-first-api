\# Application Architecture



This application follows a simple client-server architecture.



\## Main Endpoints

\- `/users/register` - User registration

\- `/users/login` - User login

\- `/restaurants` - Get restaurants list

\- `/reservations` - Create reservation



\## Architecture Diagram



```mermaid

flowchart TD

&#x20;   A\[User] --> B\[Client / Browser / Postman]

&#x20;   B --> C\[Node.js + Express REST API]



&#x20;   C --> D\[/users/register/]

&#x20;   C --> E\[/users/login/]

&#x20;   C --> F\[/restaurants/]

&#x20;   C --> G\[/reservations/]



&#x20;   D --> H\[(MariaDB Database)]

&#x20;   E --> H

&#x20;   F --> H

&#x20;   G --> H

```



\## Database Tables

\- users

\- restaurants

\- reservations

