# EXPERIMENT--01-ALP-FOR-8086
#Name : LOKESHVARAN S
#Roll no : 212223040105





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
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC Loop
INC CL
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT 
```


## Output  
 ![ADD](https://github.com/user-attachments/assets/04543ec2-2407-4aeb-bc6b-65d6685e1b50)

## Subtraction   of 8 bit numbers  ALP 
 ```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
SUB AX,BX
JNC Loop
INC CL  
NOT AX
INC AX
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT 
```
## Output
![SUB](https://github.com/user-attachments/assets/b3198914-c807-4421-853a-86816d8ab712)

## Multiplication alp 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT

```
 ## Output  
![MUL](https://github.com/user-attachments/assets/0604f061-abdc-4725-8bb2-1e52ec6e10b9)


## Division alp 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT

```
## Output  
![DIV](https://github.com/user-attachments/assets/92317a9c-cce6-4cdc-bf18-12932a308f98)


## Program for logical operations


## AND

## PROGRAM
```
 MOV AX,[3001H]
 MOV BX,[3003H]
 AND AX,BX
 MOV [3005H],AX
 HLT


```


## OUTPUT
<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/731c13a9-ac5f-46e5-8b3a-e13ce795df21" />

## OR


## PROGRAM
```
 MOV AX,[3001H]
 MOV BX,[3003H]
 OR AX,BX
 MOV [3005H],AX
 HLT
```
## OUTPUT
<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/4fef3bd8-3572-4506-be55-8ffc26729f4b" />

## NOR

## PROGRAM
```

 MOV AX,[3001H]
 MOV BX,[3003H]
 OR AX,BX  
 NOT AX
 MOV [3005H],AX
 HLT

```

## OUTPUT
<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/7142cf67-6fd0-452e-b14a-87633c4d8053" />
## NOT


## PROGRAM

```
MOV AX,[3001H]
NOT AX
MOV [3003H],AX
HLT
```

## OUTPUT

<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/fb9e4566-0944-484a-8157-a8e2ea0ea4cc" />

## XOR


## PROGRAM
```
MOV AX,[3001H]
 MOV BX,[3003H]
 XOR AX,BX
 MOV [3005H],AX
 HLT

```
## OUTPUT

<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/b4ff01a9-d8df-4828-8b7c-868f0ca1e8c3" />

## XNOR

## PROGRAM
```
 MOV AX,[3001H]
 MOV BX,[3003H]
 XOR AX,BX
 NOT AX
 MOV [3005H],AX
 HLT
```
## OUTPUT
<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/bfc3c979-cfb7-4b50-aaae-7559d69ccae8" />

## NAND

## PROGRAM
```
 MOV AX,[3001H]
 MOV BX,[3003H]
 AND AX,BX
NOT AX
 MOV [3005H],AX
 HLT
```
## OUTPUT
<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/54752a8c-7694-4eb6-99a0-2a37250b3878" />

## Result :
 

Thus the given arithmetic and logical operations have been successfully executed.





