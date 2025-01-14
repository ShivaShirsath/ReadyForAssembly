# Assembly

> Program :

```asm
DATA SEGMENT

     MSG DB "Hello World !$"
     
DATA ENDS

CODE SEGMENT  
    ASSUME DS:DATA, CS:CODE
    
    START:
        MOV AX, DATA
        MOV DS, AX
        
            LEA DX, MSG
            MOV AH, 9
            INT 21H
        
        MOV AH, 4CH
        INT 21H
        
CODE ENDS

    END START
```

> How To Run :

* Exit to terminal
* Use `EDIT` command for creating / editing `.ASM` file as below
   + `EDIT MAIN.ASM`
* Save Edited file & Exit to terminal
* Use `TASM` command for making the assembly code to object code ( `.ASM` to `.OBJ` ) as below
   + `TASM MAIN.ASM`
* Use `TLINK` command for linking the object code to executable code ( `.OBJ` to `.EXE` ) as below
   + `TLINK MAIN.OBJ`
* Use file name with extension `.EXE` for Running the Executable file as below
   + `MAIN.EXE`

> OutPut :

![Output](output.png)

<h2 align=center><a href=DOS%20Box_1.1.1.apk?raw=true>⇩ DOS Box ⇩<br>For Android</a></h2>
 <h2 align=center><a href=TC.zip?raw=true>⇩ Required Files ⇩<br>(Extract to phone storage)<br>For Android</a></h2>
<h2 align=center><a href=Assembler.apk?raw=true>⇩  Assembler ⇩<br>For Android</a></h2>


