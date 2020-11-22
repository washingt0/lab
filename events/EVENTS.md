
| Event                     | Publisher         | Published When                                                                                                                                |
|---------------------------|-------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
| `USER_CREATED`            | IAM               | A new user is created                                                                                                                         |
| `USER_DELETED`            | IAM               | A user requested account removal                                                                                                              |
| `SESSION_CREATED`         | IAM               | A user performed a sign-in and a session was issued                                                                                           |
| `SESSION_UPDATED`         | IAM               | A user-related data has changed so all his session may have to be updated                                                                     |
| `SESSION_REVOKED`         | IAM               | A session was terminated by the user or administrator command                                                                                 |
| `REQUIRE_SESSIONS`        | *                 | Any service that needs to get all current available session can emit this event and as response IAM should emit `SESSION_UPDATED` events      |
| `TRADING_FILE_RECEIVED`   | B3                | A user has uploaded a trading file for further processing                                                                                     |
| `SYMBOL_UPDATED`          | B3                | New info about the symbol was gathered                                                                                                        |
| `NEW_TRADE_OPERATION`     | B3                | A new trade operation is received                                                                                                             |
