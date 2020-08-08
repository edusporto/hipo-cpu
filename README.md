# hipo-cpu
CPU inspired by the HIPO design created in Logisim for the MAC0329 course @ IME-USP

## Authors

* **Eduardo Sandalo Porto - 11796510** - (https://github.com/edusporto)
* **João Henri Carrenho Rocha - 11796378** - (https://github.com/jaehnri)

## Instruction set

This CPU assumes 16 bit instructions, in which the first 8 bits will be an instruction and the following 8 bits are its complement.

EE means the instruction's complement and AC is the accumulator register.

| Code  | Description                                |
| ----: | ------------------------------------------ |
|  00   | NOP (no operation)                         |
|  01   | Copy [EE] to [AC]                          |
|  02   | Copy [AC] to address EE                    |
|  03   | Add [EE] to [AC] and store in AC           |
|  04   | Subtract [EE] from [AC] and store in AC    |
|  07   | Read from keyboard and store in address EE |
|  08   | Print [EE]                                 |
|  09   | Stop                                       |
|  0A   | Jump to EE                                 |
|  0B   | Jump to EE if [AC] > 0                     |
|  0D   | Jump to EE if [AC] = 0                     |

## Loading programs

Right click the RAM in Logisim and select the option to load content. There are tests programs in the `tests` directory.
