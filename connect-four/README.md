# Connect Four

Connect Four is a classic board game. See [https://en.wikipedia.org/wiki/Connect_Four](https://en.wikipedia.org/wiki/Connect_Four) for an overview.

See [interface.proto](interface.proto) for the gRPC interface your agent needs to implement.

### Rules

 * The game is played on the classic board with 7 columns and 6 rows.
 * The game proceeds in turns alternating between two agents. On each turn an agent plays a stone in a column.
 * A move is invalid if it's outside the range 0-6, or 6 stones have already been played in the column. If your agent plays an invalid move, it immediately loses.  
 * The game is won when an agent manages to connect four stones, either vertically, horizontally or diagonally.
 * The game is a draw if the board is full (42 moves), and there's no winner.

 
### Example agents

 * [Java](https://github.com/battleai/agents.java)
