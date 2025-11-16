# Snake Game 🐍

A classic Snake game implementation in C++ using console graphics. Control the snake to eat food and grow longer while avoiding collisions with walls and yourself!

## 📋 Project Description

This is a console-based Snake game written in C++ that runs on Windows. The player controls a snake that moves around the screen, eating food to grow longer. The objective is to achieve the highest score possible by consuming as much food as you can without hitting the boundaries or the snake's own body.

## 👥 Team Members

- **Tran Nguyen Thuan Phat** - 24521319
- **Cao Minh Huy** - 24520652
- **Duong Tu Thanh** - 24521619

## 🎮 Features

- Simple and intuitive keyboard controls
- Dynamic snake growth upon eating food
- Random food generation
- Console-based graphics using ASCII characters
- Real-time gameplay with adjustable speed

## 🕹️ How to Play

### Controls

- **W** - Move Up
- **A** - Move Left
- **S** - Move Down
- **D** - Move Right

### Gameplay

1. The snake starts with a length of 3 segments
2. Food (`*`) appears randomly on the screen
3. Navigate the snake (`X` characters) to eat the food
4. Each food item increases the snake's length by 1
5. Avoid hitting the boundaries (defined by MINX, MINY, MAXX, MAXY)

## 🔧 Requirements

- **Operating System**: Windows
- **Compiler**: C++ compiler with C++11 support or higher (e.g., MinGW, MSVC)
- **Libraries**:
  - `windows.h` (for console manipulation)
  - `conio.h` (for keyboard input)

## 🚀 Compilation and Execution

### Using g++ (MinGW)

```bash
g++ main.cpp -o snake.exe
snake.exe
```

### Using Visual Studio

1. Create a new C++ Console Application project
2. Replace the default code with `main.cpp`
3. Build and run the project (F5)

## 📝 Code Structure

### Classes and Structures

#### `Point`

- Simple structure to store x, y coordinates

#### `CONRAN` (Snake Class)

- **Attributes**:
  - `Point A[100]`: Array storing snake segments
  - `int DoDai`: Current length of the snake
- **Methods**:
  - `CONRAN()`: Constructor initializing snake with length 3
  - `void Ve(Point Qua)`: Renders the snake and food on screen
  - `void DiChuyen(int Huong, Point &Qua)`: Moves the snake in specified direction
  - `void AnMoi(Point Qua)`: Handles food consumption and growth

### Functions

- `void gotoxy(int column, int line)`: Positions the cursor at specified coordinates
- `int main()`: Main game loop handling input, rendering, and game logic

## 🎯 Game Constants

- `MINX = 2`: Minimum X boundary
- `MINY = 2`: Minimum Y boundary
- `MAXX = 35`: Maximum X boundary
- `MAXY = 20`: Maximum Y boundary

## 🔄 Game Loop

1. Check for keyboard input
2. Clear the screen
3. Render snake and food
4. Move snake in current direction
5. Check for food collision and update
6. Wait 300ms before next iteration

## 🛠️ Future Improvements

- Add collision detection with walls and self
- Implement scoring system
- Add difficulty levels with varying speeds
- Create a game over screen
- Add high score tracking
- Implement pause functionality
- Add visual enhancements with borders

## 📜 License

This project is created for educational purposes.

## 🤝 Contributing

This is a student project. Feedback and suggestions are welcome!

---

**Developed as part of a programming course project**
