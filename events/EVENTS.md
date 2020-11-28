
| Event                     | Queue             | Publisher         | Published When                                                                                                                                |
|---------------------------|-------------------|-------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
| `USER_CREATED`            | `USER`            | IAM               | A new user is created                                                                                                                         |
| `USER_DELETED`            | `USER`            | IAM               | A user requested account removal                                                                                                              |
| `SESSION_CREATED`         | `SESSION`         | IAM               | A user performed a sign-in and a session was issued                                                                                           |
| `SESSION_UPDATED`         | `SESSION`         | IAM               | A user-related data has changed so all his session may have to be updated                                                                     |
| `SESSION_REVOKED`         | `SESSION`         | IAM               | A session was terminated by the user or administrator command                                                                                 |
| `REQUIRE_SESSIONS`        | `IAM`             | *                 | Any service that needs to get all current available session can emit this event and as response IAM should emit `SESSION_UPDATED` events      |
| `TRADING_FILE_RECEIVED`   | `TRADE`           | B3                | A user has uploaded a trading file for further processing                                                                                     |
| `NEW_TRADE_OPERATION`     | `TRADE`           | B3                | A new trade operation is received                                                                                                             |
| `SYMBOL_UPDATED`          | `SYMBOL`          | B3                | New info about the symbol was gathered                                                                                                        |
