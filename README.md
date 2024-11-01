# ft_printf

# ft_printf Project

![Build Status](https://img.shields.io/badge/build-passing-brightgreen) ![License](https://img.shields.io/badge/license-MIT-blue) ![Language](https://img.shields.io/badge/language-C-blue)

**ft_printf** is a 42 School project that involves recreating the standard `printf` function in C. I implemented my own version, called **ft_printf**, which supports various formatting types such as integers, characters, strings, hexadecimal numbers, and pointers. This project allowed me to deepen my understanding of variadic functions, memory management, and output formatting in C.

The **ft_printf** project requires the creation of a function that replicates the behavior of the standard `printf` function. My implementation, **ft_printf**, supports different types of formatting and focuses on:
- **Variadic Functions Management**: Using variadic functions (`va_list`, `va_start`, `va_arg`, `va_end`) to accept a variable number of arguments.
- **Output Formatting**: Support for format specifiers such as `c`, `s`, `d`, `i`, `u`, `x`, `X`, `p`, and `%`.
- **Memory Management**: Allocating and managing memory to produce formatted output according to the specified format specifiers.

---

**ft_printf** è un progetto della 42 School che consiste nel ricreare la funzione standard `printf` in C. Ho implementato la mia versione, chiamata **ft_printf**, che supporta diversi tipi di formattazione, come interi, caratteri, stringhe, numeri esadecimali e puntatori. Questo progetto mi ha permesso di approfondire l'uso delle variadic functions, la gestione della memoria e la formattazione dell'output in C.

Il progetto **ft_printf** richiede la realizzazione di una funzione che replica il comportamento della funzione `printf` standard. La mia implementazione, **ft_printf**, supporta vari tipi di formattazione e si concentra su:
- **Gestione delle Variadic Functions**: Utilizzo di variadic functions (`va_list`, `va_start`, `va_arg`, `va_end`) per accettare un numero variabile di argomenti.
- **Formattazione dell'Output**: Supporto per specificatori di formato come `c`, `s`, `d`, `i`, `u`, `x`, `X`, `p` e `%`.
- **Gestione della Memoria**: Allocazione e gestione della memoria per generare output formattato in base agli specificatori.

---

## Features

| Specifier           | Description                                                                                          |
|---------------------|------------------------------------------------------------------------------------------------------|
| **%c**              | 🇬🇧 Prints a single character.<br>🇮🇹 Stampa un singolo carattere.                                     |
| **%s**              | 🇬🇧 Prints a string of characters.<br>🇮🇹 Stampa una stringa di caratteri.                              |
| **%d / %i**         | 🇬🇧 Prints a decimal (base 10) integer.<br>🇮🇹 Stampa un intero decimale (base 10).                     |
| **%u**              | 🇬🇧 Prints an unsigned decimal integer.<br>🇮🇹 Stampa un intero decimale senza segno.                    |
| **%x / %X**         | 🇬🇧 Prints a hexadecimal (base 16) integer in lowercase or uppercase.<br>🇮🇹 Stampa un intero esadecimale (base 16) in minuscolo o maiuscolo. |
| **%p**              | 🇬🇧 Prints a pointer address in hexadecimal format.<br>🇮🇹 Stampa un indirizzo di puntatore in formato esadecimale. |
| **%%**              | 🇬🇧 Prints a percentage symbol.<br>🇮🇹 Stampa un simbolo di percentuale.                                 |

---

## Functions

| Function              | Description                                                                                         |
|-----------------------|-----------------------------------------------------------------------------------------------------|
| `ft_printf.c`         | 🇬🇧 Main function to handle formatted output based on format specifiers.<br>🇮🇹 Funzione principale per gestire l'output formattato in base agli specificatori di formato. |
| `ft_putchar.c`        | 🇬🇧 Outputs a single character to the standard output.<br>🇮🇹 Stampa un singolo carattere su standard output. |
| `ft_putstr.c`         | 🇬🇧 Outputs a string to the standard output.<br>🇮🇹 Stampa una stringa su standard output.            |
| `ft_putnbr.c`         | 🇬🇧 Outputs an integer to the standard output, handling negative numbers.<br>🇮🇹 Stampa un intero su standard output, gestendo i numeri negativi. |
| `ft_unsigned_putnbr.c`| 🇬🇧 Outputs an unsigned integer to the standard output.<br>🇮🇹 Stampa un intero senza segno su standard output. |
| `ft_hex_putnbr.c`     | 🇬🇧 Outputs an integer in hexadecimal format (lowercase or uppercase).<br>🇮🇹 Stampa un intero in formato esadecimale (minuscolo o maiuscolo). |
| `ft_meetperc.c`       | 🇬🇧 Processes each format specifier and directs output accordingly.<br>🇮🇹 Gestisce ogni specificatore di formato e invia l'output di conseguenza. |

---

## Compilation and Usage

🇬🇧
| Step                       | Description                                                                                                                  |
|----------------------------|------------------------------------------------------------------------------------------------------------------------------|
| **Compilation**            | Compile the library by running `make`. This will generate the object files (`.o`) that can be linked to other projects.      |
| **Including Header**       | Include the `ft_printf.h` file in your source code to access the **ft_printf** function.                                     |
| **Linking**                | Compile your project with **ft_printf** by linking the files. For example:<br> `gcc your_program.c ft_printf.c ft_putchar.c ft_putstr.c ft_putnbr.c ft_unsigned_putnbr.c ft_hex_putnbr.c ft_meetperc.c -o your_program` |
| **Use in Any Project**     | You can use **ft_printf** in any project simply by including `ft_printf.h` and linking the compiled library during compilation. This way, you don't need a specific main function for **ft_printf** inside the library. Include `ft_printf.h` in the source files where you want to use **ft_printf**. |
| **Example Usage**          | Inside your program, you can use **ft_printf** like the standard `printf`.                                                   |

---

🇮🇹 

| Passaggio                 | Descrizione                                                                                                                   |
|---------------------------|-------------------------------------------------------------------------------------------------------------------------------|
| **Compilazione**          | Compila la libreria eseguendo `make`. Questo genererà i file oggetto (`.o`) che possono essere collegati ad altri progetti.   |
| **Inclusione dell'Header**| Includi il file `ft_printf.h` nel tuo codice sorgente per accedere alla funzione **ft_printf**.                              |
| **Collegamento**          | Compila il tuo progetto insieme a **ft_printf** collegando i file. Ad esempio:<br> `gcc your_program.c ft_printf.c ft_putchar.c ft_putstr.c ft_putnbr.c ft_unsigned_putnbr.c ft_hex_putnbr.c ft_meetperc.c -o your_program` |
| **Utilizzo in Qualsiasi Progetto** | Puoi utilizzare **ft_printf** in qualsiasi progetto semplicemente includendo `ft_printf.h` e collegando la libreria compilata durante la compilazione. In questo modo, non hai bisogno di un `main` specifico per **ft_printf** all'interno della libreria. Includi `ft_printf.h` nei file sorgente del progetto dove vuoi usare **ft_printf**. |
| **Esempio di Utilizzo**   | All'interno del tuo programma, puoi usare **ft_printf** come la funzione `printf` standard.                                   |

---
