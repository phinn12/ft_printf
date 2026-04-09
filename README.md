# ft_printf

`ft_printf` is a custom implementation of the standard `printf` function from the 42 curriculum. This version builds as a static library and supports the core mandatory conversion set.

## Supported conversions

From the current implementation in [`ft_printf.c`](ft_printf.c):

- `%c`
- `%s`
- `%p`
- `%d`
- `%i`
- `%u`
- `%x`
- `%X`
- `%%`

## Build

```bash
make
```

This creates:

```text
libftprintf.a
```

## Use it in another C project

Compile the library:

```bash
make
```

Then link it:

```bash
cc your_program.c libftprintf.a -o your_program
```

## Public API

Declared in [`ft_printf.h`](ft_printf.h):

```c
int	ft_printf(const char *str, ...);
```

Helper functions in the same library include:

- `ft_putchar`
- `ft_putstr`
- `ft_putptr`
- `ft_putnbr`
- `ft_puthex`

## Project files

```text
ft_printf/
├── ft_printf.c
├── ft_printf_utils.c
├── ft_printf.h
└── Makefile
```

## Verified during this documentation pass

- `make` completed successfully
- `libftprintf.a` was generated correctly
