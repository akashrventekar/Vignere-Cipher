# Vignere-Cipher
C program which demonstrates Vignere Cipher encryption and decryption

Instructions:

1) Compile Source code: cc Source.c

av0018@dakota:~/Vignere Cipher$ cc Source.c 
Source.c: In function ‘main’:
Source.c:33:3: warning: incompatible implicit declaration of built-in function ‘exit’ [enabled by default]
   exit(1); //Exit the program 
   ^
Source.c:50:3: warning: incompatible implicit declaration of built-in function ‘exit’ [enabled by default]
   exit(1);
   ^
Source.c:64:3: warning: incompatible implicit declaration of built-in function ‘exit’ [enabled by default]
   exit(1);
   ^
Source.c: In function ‘encode’:
Source.c:120:2: warning: format not a string literal and no format arguments [-Wformat-security]
  fprintf(fp2, cipher);
  ^
Source.c: In function ‘decode’:
Source.c:168:2: warning: format not a string literal and no format arguments [-Wformat-security]
  fprintf(fp2, message);
  ^

2) Make sure that the Input file (containing message or cipher text) and the file containing user supplied key exist.
  
3) Execute the code: ./a.out

av0018@dakota:~/Vignere Cipher$ ./a.out

Sample Input and Output:
Press 0 to encode, 1 to decode,anythin else to exit
0
Enter the input filename containing not more than 1024 upper-case characters: Message.txt
Enter the filename containing the key not more than 1024 upper-case characters: Key.txt
Key : AAAAA
Message:    SECURITY
Final key:  AAAAAAAA
Ciphertext: SECURITY
Message.txt.v created

av0018@dakota:~/Vignere Cipher$ ./a.out
Press 0 to encode, 1 to decode,anythin else to exit
1
Enter the input filename containing not more than 1024 upper-case characters: Mess.txt.v
Enter the filename containing the key not more than 1024 upper-case characters: Key.txt
Key : AAAAA
Ciphertext: ABCDEFGHIJKLMNOPQRSTUVWXYZ
Final key:  AAAAAAAAAAAAAAAAAAAAAAAAAA
Message:    ABCDEFGHIJKLMNOPQRSTUVWXYZ
Message.txt created

av0018@dakota:~/Vignere Cipher$ ./a.out
Press 0 to encode, 1 to decode,anythin else to exit
0
Enter the input filename containing not more than 1024 upper-case characters: Mess.txt   
Enter the filename containing the key not more than 1024 upper-case characters: Key.txt
Key : AAAAA
Message:    ABCDEFGHIJKLMNOPQRSTUVWXYZ
Final key:  AAAAAAAAAAAAAAAAAAAAAAAAAA
Ciphertext: ABCDEFGHIJKLMNOPQRSTUVWXYZ
Mess.txt.v created

av0018@dakota:~/Vignere Cipher$ ./a.out
Press 0 to encode, 1 to decode,anythin else to exit
1
Enter the input filename containing not more than 1024 upper-case characters: Message.txt.v
Enter the filename containing the key not more than 1024 upper-case characters: Key.txt
Key : AAAAA
Ciphertext: SECURITY
Final key:  AAAAAAAA
Message:    SECURITY
Message.txt created

av0018@dakota:~/Vignere Cipher$ ./a.out
Press 0 to encode, 1 to decode,anythin else to exit
0
Enter the input filename containing not more than 1024 upper-case characters: me
sssss
messsss File does not exist


Few exceptions handled:
Invalid Input 
File not found
White space removal
Conversion from lowercase to upper case

