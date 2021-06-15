# Data types

| Name | Bits | Data and Ranges                                          | Equivalent in C language |
| ---- | ---- | -------------------------------------------------------- | ------------------------ |
| i8   | 8    | [-128 - 127]                                             | signed char = int8_t     |
| i16  | 16   | [-32,768 - 32,767]                                       | short = int16_t          |
| i32  | 32   | [-2,147,483,648 - 2,147,483,647]                         | int = int32_t            |
| i64  | 64   | [-9,223,372,036,854,775,808 - 9,223,372,036,854,775,807] | long long = int64_t      |
| i128 | 128  |                                                          |                          |
| u8   | 8    | 0-255                                                    | uint8_t                  |
| u16  | 16   | [0-65535]                                                | uint16_t                 |
| u32  | 32   | [0-4294967295]                                           | uint32_t                 |
| u64  | 64   | [0-18446744073709551615]                                 | uint64_t                 |
| u128 | 128  |                                                          |                          |

Source of C language:

- <https://gcc.gnu.org/onlinedocs/gcc/_005f_005fint128.html>
- <https://os.mbed.com/handbook/C-Data-Types>
- <https://www.badprog.com/c-type-what-are-uint8-t-uint16-t-uint32-t-and-uint64-t>
- <https://ro-che.info/articles/2017-01-25-word8-space>
