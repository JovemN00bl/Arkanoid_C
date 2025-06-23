# Arkanoid in C with SDL2

![Status](https://img.shields.io/badge/status-functional-green)
![Language](https://img.shields.io/badge/language-C-blue)
![Library](https://img.shields.io/badge/library-SDL2-red)
![Platform](https://img.shields.io/badge/platform-Linux-orange)

A classic Arkanoid clone written from scratch in C. This project uses the **SDL2** library for 2D graphics rendering and window management, and **Pthreads** for concurrent input handling.

This project serves as a practical demonstration of game development in C on Linux, covering graphics, user input, game logic, and concurrency.

<br>



## ✨ Features

-   **Classic Gameplay:** Control a paddle at the bottom of the screen to bounce a ball and destroy all the bricks.
-   **Graphics with SDL2:** All rendering (paddle, ball, bricks, score) is handled using the SDL2 library.
-   **Score and Lives System:** Keep track of your score as you destroy bricks and manage your three lives.
-   **Concurrent Input:** User input is handled on a separate thread using Pthreads, ensuring smooth gameplay and responsive controls without blocking the main game loop.
-   **Real-time Physics:** Simple physics for ball movement and collision detection with walls, the paddle, and bricks.

---

## 🛠️ Core Technologies

-   **Language:** C
-   **Libraries:**
    -   **SDL2:** A cross-platform development library for low-level access to audio, keyboard, mouse, joystick, and graphics hardware.
    -   **Pthreads:** The standard POSIX Threads library for managing concurrency.
    -   **Standard C Libraries** (`stdlib.h`, `string.h`, `unistd.h`).

---

## ⚙️ Prerequisites

To compile and run this project, you will need:

-   **Operating System:** A Linux environment (like Ubuntu, Debian, etc.) or a subsystem like WSL.
-   **Compiler:** **GCC** (GNU Compiler Collection).
-   **SDL2 Development Library:** The `libsdl2-dev` package.

You can install the necessary dependencies on a Debian/Ubuntu-based system with the following command:
```bash
sudo apt update && sudo apt install build-essential libsdl2-dev
```



## 🚀 How to Compile


1.  **Compile the Project:**
    Use GCC to compile the source code. The `-lSDL2` and `-lpthread` flags are required to link the SDL2 and Pthread libraries, respectively.
    ```bash
    gcc main.c -o arkanoid -lSDL2 -lpthread
    ```

---
