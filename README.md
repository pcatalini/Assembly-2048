# 2048 ASSEMBLY FOR 8086 ARCHITECTURE 

![alt text](/img/2048.jpg)

## About the project

This program was developed to learn instructions of 8086 processor, it was a task for the Computer engineer course at university of PUC Campinas brazil.

## How i can run it?

It will be necessary to run inside a DOS environment, of course it's not easy to find a original computer with DOS on now's days, however we can do that by using virtual machine like DOSBOX

## Steps to setup enviroment
1. First download the [DOSBOX](https://www.dosbox.com/download.php?main=1) and follow the official documentation to install it;
1. It will be necessary to mount a volume from the host machine into the DOSBOX, for that, use the command bellow
    ```dos
    MOUNT C PATH_ROOT_PROJECT
    ```
    Change the PATH_ROOT_PROJECT with the path for your root project within your host computer

1. Now you can enter into the directory by typing

    ```dos
    C: C
    ```
    By performing the `<dir>` command you should be able to see the files from that mouted point

## Steps to compile the project

1. To compile we'll use two auxiliary programs, which are `TASM.EXE` and `TLINK.EXE`. both of them is insie root folder of this project. to convert the .ASM into a .OBJ run the following command
    ```dos
    TASM.EXE 2048.ASM
    ```
    By typing the command `<dir>` again you should be able to see the 2048.OBJ as an output from the command above.

1. To compile and generates an .EXE it will be required to use TLINK.EXE program as shown bellow
    ```dos
    TLINK.EXE 2048.obj
    ```

1.  Well done! at this point 2048 is already compiled! to run it use the following command
    ```dos
    2048.EXE
    ```
## Other informations
The performance can be increased by typing the keys `Ctrl+f12` or decrease using `Ctrl+f11`, it is recommended to decrease velocity at least once to check what is happening on the screen during the screen print process
