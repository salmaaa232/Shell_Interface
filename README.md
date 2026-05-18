<div align="center">

# Web Shell Interface

**Browser-based shell with a simulated filesystem** &mdash; run familiar Unix-style commands with history, tab completion, and a dark terminal UI.

<br>

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=000)](https://developer.mozilla.org/docs/Web/JavaScript)
[![No install](https://img.shields.io/badge/Install-none-22c55e?style=for-the-badge)]()

<br>

[Quick start](#quick-start) &middot; [Commands](#command-reference) &middot; [Contributors](#contributors)

</div>

---

## Table of contents

| | |
| :-- | :-- |
| **Run it** | [Quick start](#quick-start) |
| **Reference** | [Command reference](#command-reference) &middot; [UI](#interface) |
| **Project** | [Structure](#project-structure) &middot; [Technical notes](#technical-notes) |
| **Team** | [Contributors](#contributors) |

---

## Quick start

1. Clone or download this repository.
2. Open **`web_shell.html`** in any modern browser (double-click or *File &rarr; Open*).
3. Type commands in the prompt; press **Enter** to run.

No build step, no server, and no extra dependencies.

---

## Command reference

| Command | Usage | What it does |
| :------ | :---- | :------------- |
| **ls** | `ls` &middot; `ls <path>` | List entries in the current directory or at *path* (absolute or relative). |
| **cd** | `cd <path>` | Change directory. Supports `/absolute`, relative paths, `..`, and `~` (home maps to `/`). |
| **pwd** | `pwd` | Print the current working directory. |
| **mkdir** | `mkdir <path>` | Create a directory (nested paths allowed if parents exist). |
| **rmdir** | `rmdir <path>` | Remove an **empty** directory only. |
| **touch** | `touch <file> ...` | Create empty files (or report if they already exist). |
| **rm** | `rm <file> ...` | Remove **files** only (not directories). |
| **cat** | `cat <file> ...` | Show built-in or user-created file contents. |
| **echo** | `echo <text ...>` | Print text. |
| **help** | `help` | List commands and tips. |
| **clear** | `clear` | Clear the on-screen output. |

**Keyboard:** **Up** / **Down** arrow keys for history &middot; **Tab** completes command names &middot; **Enter** runs the line.

---

## Interface

| | |
| :-- | :-- |
| **Theme** | Dark, monospace, terminal-style layout |
| **Output** | Color hints for commands, results, help, and errors |
| **Input** | Line editor with history and tab completion |
| **Layout** | Responsive; usable on desktop and smaller screens |

---

## Project structure

```
OS_Project/
+-- web_shell.html    # Single-page shell (HTML + CSS + JS)
+-- README.md         # This file
```

---

## Technical notes

- The filesystem is **simulated in memory** in the browser for demonstration.
- **Paths** behave like a small Unix tree: `.`, `..`, absolute (`/...`), and relative segments.
- **`rm`** vs **`rmdir`**: files vs empty directories; wrong tool yields realistic-style errors.
- State lasts for the **current tab session**; reloading the page resets the simulation.

---

## Contributors

<div align="center">

**Course project &mdash; team roster**

| Team member | Student ID |
| :---------- | ---------: |
| Salma Medhat | 320240082 |
| Malak Mohamed | 320240101 |
| Salma Mohamed | 320240083 |
| Maryam Ahmed | 320240105 |

</div>
