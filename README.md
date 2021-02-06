# ARM-Processor
A Pipeline implementation of ARM
## How it works ? 

This CPU has a `12bit` data bus and a `12bit` address bus.
All of the Instructions are 12 bit.
This CPU have these components : 
* 1 12bits register named Accumulator (ACC)
* 1 1bit flag named CY

This CPU has 3 groups of Instructions.

Group 0 Instructions :

| Instruction Mnemonic | Definition              | Bits 11:9 | RTL Notation                                                |
|----------------------|-------------------------|-----------|-------------------------------------------------------------|
| NOP                  | Logical AND             | 0         | ACC <- ACC & (EA);                                          |
| ADD                  | 2's complement add      | 001       | {CY, ACC} <- ACC + (EA);                                    |
| ISZ                  | Increment and skip if 0 | 010       | (EA) <- (EA) + 1; if (EA) + 1 = 0 skip the next instruction |
| DCA                  | Deposit and clear ACC   | 011       | (EA) <- ACC; ACC <- 0;                                      |
| JMP                  | Jump                    | 100       | Jump to location EA                                         |
| JMS                  | Jump to subroutine      | 101       | Jump to subroutine at location EA                           |
## Developers

* [**Mobina Shahbandeh**](https://github.com/mobinashb)
* [**Ghazal Kalhor**](https://github.com/kalhorghazal)

