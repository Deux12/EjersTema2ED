

 Ejecuta el programa "Hola mundo" en los siguientes lenguajes:
○ bash:

ivan@ivan-VirtualBox:~$ cat > hola.sh
#!/usr/bin/env bash

echo "Hola Ivan Cernadas."   
ivan@ivan-VirtualBox:~$ chmod +x hola.sh 
ivan@ivan-VirtualBox:~$ ./hola.sh 
Hola Ivan Cernadas.

○ python:


○ php:

van@ivan-VirtualBox:~$ cat > hola.php
#!/usr/bin/env php

<?php 
  echo "Hola Ivan Cernadas\n" 
?>
ivan@ivan-VirtualBox:~$ chmod +x hola.p
ivan@ivan-VirtualBox:~$ ./hola.php

Hola Ivan Cernadas

○ javascript (nodejs):

ivan@ivan-VirtualBox:~$ cat > hola.js
#!/usr/bin/env node

console.log('Hola Ivan Cernadas');
ivan@ivan-VirtualBox:~$ chmod  +x  hola.js
ivan@ivan-VirtualBox:~$ ./hola.js
Hola Ivan Cernadas

○ c:

ivan@ivan-VirtualBox:~$ cat > hola.c
#include <stdio.h>

int main()
{
    printf("¡Hola, Ivan Cernadas!");
    return 0;
}
ivan@ivan-VirtualBox:~$ gcc  -o  hola  hola.c 
ivan@ivan-VirtualBox:~$ ./hola       
¡Hola, Ivan Cernadas!

○ c++:

ivan@ivan-VirtualBox:~$ cat > hola.cpp
#include <iostream>

using namespace std;

int main()
{
   cout << "¡Hola, Ivan Cernadas!" << endl;
   return 0;
}
ivan@ivan-VirtualBox:~$ g++  -o  hola  hola.cpp 
ivan@ivan-VirtualBox:~$ ./hola  
¡Hola, Ivan Cernadas!

○ java:

ivan@ivan-VirtualBox:~$ cat > hola.java
class Hola
{
    public static void main(String[] args)
    {
        System.out.println("Hola Ivan Cernadas");
    }
}
ivan@ivan-VirtualBox:~$ javac  hola.java  
ivan@ivan-VirtualBox:~$ java -cp d:\java hola.java
Hola Mundo


○ ruby:

ivan@ivan-VirtualBox:~$ cat > hola.rb
#!/usr/bin/env ruby

puts "Hola Mundo"
ivan@ivan-VirtualBox:~$ chmod  +x  hola.rb
ivan@ivan-VirtualBox:~$ ./hola.rb
Hola Mundo

○ go:

ivan@ivan-VirtualBox:~$ cat > hola.go
package main

import "fmt"

func main() {
        fmt.Println("Hola Ivan Cernadas") 
}
ivan@ivan-VirtualBox:~$ go  run  hola.go 
Hola Ivan Cernadas


○ rust:

ivan@ivan-VirtualBox:~$ cat > hola.rs
fn main() {
    println!("¡Hola, Ivan Cernadas");     
}
ivan@ivan-VirtualBox:~$ rustc  hola.rs 
ivan@ivan-VirtualBox:~$ ./hola
¡Hola, Ivan Cernadas

○ lisp:

ivan@ivan-VirtualBox:~$ cat > hola.lisp
#!/usr/bin/env clisp

(format t "¡Hola, Ivan Cernadas")
ivan@ivan-VirtualBox:~$ chmod  +x  hola.lisp
ivan@ivan-VirtualBox:~$ 
ivan@ivan-VirtualBox:~$ ./hola.lisp
¡Hola, Ivan Cernadas

○ ensamblador (nasm):

ivan@ivan-VirtualBox:~$ cat > hola.asm
 section .data
 
 msg     db "¡Hola, Ivan Cernadas", 0Ah
 len     equ     $ - msg  
 
 section .text
 
 global _start
 
 _start:
        mov     eax, 04h
        mov     ebx, 01h
        mov     ecx, msg
        mov     edx, len
        int     80h
        mov     eax, 01h
        mov     ebx, 00h
        int     80h
ivan@ivan-VirtualBox:~$ nasm  -f  elf64  hola.asm 
ivan@ivan-VirtualBox:~$ ./hola
¡Hola, Ivan Cernadas




