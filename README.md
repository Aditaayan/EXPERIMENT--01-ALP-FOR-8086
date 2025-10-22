# EXPERIMENT--01-ALP-FOR-8086

Name : Aditaayan M

Roll no : 212223040006

## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)


9.	Click on emulate to start emulation 


![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)



10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 


![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)



## Programs for arithmetic  operations

## Addition  of 8 bit ALP 

```
org 100h

MOV AL, [4000H]
MOV BL, [4001H]
ADD AL, BL
MOV [4002H], AL

ret
```

## Output  

<img width="1919" height="1014" alt="add" src="https://github.com/user-attachments/assets/44f6e584-22a8-4984-9525-2fd200ccbd95" />

## Subtraction   of 8 bit numbers  ALP 

```
org 100h

MOV AL, 97H
MOV BL, 76H
SUB AL, BL
MOV [4000H], AL


ret
```

## Output  

<img width="1916" height="1069" alt="sub" src="https://github.com/user-attachments/assets/aafe95fc-1eb8-49f4-8e2c-6f784f861ad2" />

## Multiplication alp 

```
org 100h

MOV AL, [4400H]
MOV BL, [4401H]
MUL BL
MOV [4402H],AL
MOV [4403], AH

ret
```

## Output  

<img width="1919" height="1075" alt="mul" src="https://github.com/user-attachments/assets/2be3dde2-21b5-4c8e-a620-50f2e7368ba4" />

## Division alp 

```
org 100h

MOV AL, [4300H]
MOV BL, [4301H]
DIV BL
MOV [4302H], AL
MOV [4303H], AH

ret
```

## Output  

<img width="1919" height="1078" alt="div" src="https://github.com/user-attachments/assets/9b014b82-1056-4556-a072-4823501e8eed" />


## Program for logical operation

```
org 100h

MOV AX, 0A32H
MOV BX, 0B31H
MOV SI, 5000H
OR AX, BX
MOV [SI], AX
MOV AX, 0A32H
AND AX, BX
MOV [SI+2], AX
MOV AX, 0A32H
XOR AX, BX
MOV [SI+4], AX
MOV AX, 0A32H
NOT AX
MOV [SI+6], AX


ret
```

## Output

<img width="1918" height="1018" alt="log" src="https://github.com/user-attachments/assets/e9317ad7-cae2-49f7-b5e4-302365f20533" />

## Result :

Thus, ALP on fundamental arithmetic and logical operations is written and executed successfully.
