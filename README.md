# TIC-TAC-TOE-Console-OO

The OO version of this simple Tic-Tac-Toe is more complex than the non-OO version,
because Tic-Tac-Toe is a rather simple application. But OO design is a necessity
to build a complex application.

- The Seed and State enum classes help to store an enumeration (list) of fixed items.
- The Cell class has an instance variable called content (with package access), of the type enum Seed.
    You can only assign a value from the enum's constants, such as Seed.NO_SEED, Seed.CROSS, and
    Seed.NOUGHT, into content. A Cell can paint() itself. You can use newGame() to reset all its properties,
    ready for a new game.
- The Board class composes of nine Cell instances, arranged in an 3×3 array called cells
    (with package access), of the type Cell[][]. A Board can paint() itself, and supports
    the state transition functions such as  initGame(), newGame() and stepGame() (see game state diagram).
- GameMain acts as the overall controller for the game.