# Architecture Decision Record: Database Storage

## Summary
Determine if the mobile app Tic-Tac-Toe requires a database to save any information.

## Issue
This game does not have to save player data, scores, or history. It is an in-the-moment type of game with no need for long-term data storage.

## Decision
Decided not to use database storage.

## Status
Decided on no database. Open to adding simple local storage only if it becomes required later on.

## Details

### Assumptions
- The game is not required to save results after closing the app.  
- No user accounts and no profiles exist.

### Constraints
- A backend or local storage system is unnecessary for such a simple game.

### Positions
The other options we considered were: local storage, encrypted storage, remote database, and no storage.  
No storage is required for the functionality of this application.

### Argument
This is a game of Tic-Tac-Toe where, after each round, everything resets; it doesn't require saved data. Using a database would involve extra, unnecessary work for the team.

### Implications
- Faster development  
- No backend issues  
- No saved game history (not required)

## Related
- No extra setup needed in React Native
