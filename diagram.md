|---------------------+ +---------------+ +----------------------|
| Customer | | Contact | | Movie |
|---------------------| |---------------| |----------------------|
| CustomerID (PK) | | ContactID (PK)| | MovieID (PK) |
| Name | | Email | | Title |
| | | Phone | | Genre |
+---------------------+ +---------------+ | Duration |
| | Description |
| +----------------------+
| ^
| |
v |
+---------------------+ +---------------------+ |
| Ticket | | Showtime | |
|---------------------| |---------------------| |
| TicketID (PK) | | ShowtimeID (PK) | |
| CustomerID (FK) | | MovieID (FK) | |
| ContactID (FK) | | ScreenID (FK) | |
| ShowtimeID (FK) | | Date | |
| Booking Date | | Time | |
| Delivery Status | +---------------------+ |
+---------------------+ |
|
+---------------------+ +---------------------+ |
| Admin | | AdminMovie | |
|---------------------| |---------------------| |
| AdminID (PK) | | AdminMovieID (PK) | |
| Name | | AdminID (FK) | |
| Role | | MovieID (FK) | |
+---------------------+ +---------------------+ |
| |
v |
+---------------------+ +---------------------+ |
| AdminMovie | | Screen | |
|---------------------| |---------------------| |
| AdminMovieID (PK) | | ScreenID (PK) | |
| AdminID (FK) | | Capacity | |
| MovieID (FK) | +---------------------+ |
+---------------------+
