# ARM-Processor
A Pipeline implementation of ARM
## How it works ? 

This CPU has a `32bit` data bus and a `32bit` address bus.

All of the Instructions are 32 bit.

Instructions :

| Instruction Mnemonic | Definition          | Bits 27:26 | Bits 24:21 | 
|----------------------|---------------------|------------|------------|
| MOV                  | Move                | 00         | 1101       | 
| MVN                  | Move NOT            | 00         | 1111       | 
| ADD                  | Add                 | 00         | 0100       |
| ADC                  | Add with Carry      | 00         | 0101       |
| SUB                  | Subtract            | 00         | 0010       | 
| SBC                  | Subtract with Carry | 00         | 0110       | 
| AND                  | Logical AND         | 00         | 0000       | 
| ORR                  | Logical OR          | 00         | 1100       | 
| EOR                  | Exclusive OR        | 00         | 0001       | 
| CMP                  | Compare             | 00         | 1010       |
| TST                  | Test                | 00         | 1000       | 
| LDR                  | Load Register       | 01         | 0100       | 
| STR                  | Store Register      | 01         | 0100       | 
| B                    | Branch              | 10         | XXXX       | 
## Developers

* [**Mobina Shahbandeh**](https://github.com/mobinashb)
* [**Ghazal Kalhor**](https://github.com/kalhorghazal)
