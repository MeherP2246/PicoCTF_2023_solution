# Cryptography 
_____________________________________________________________________________________________________________________________________________________


## HideToSee

![image](https://github.com/MeherP2246/PicoCTF_2023_solution/assets/134104519/77a9a054-8cad-42f4-8d00-4caeacb85261)

### Solution: 
Step1 : Download the image file (atbash.jpg) and use steghide to extract the hidden information 

```sudo apt-get install steghide -y```

Step 2: After downloading the steghide run the below commad

```steghide extract -sf atbash.jpg```

Result : It will extracted data  and store it into  "encrypted.txt" file.

Step 3 : Open the "encrypted.txt" file using 

```cat encrypted.txt ```
 
 
Result : krxlXGU{zgyzhs_xizxp_1u84w779}

We know this is not the actual flag , but if we look close to the atbash.jpg image will get know that the atbash is the cipher used for encryption.

simply go the google and search for atbash cipher decoder and decode the above cipher, we will get the final flag.


 ### FLag : picoCTF{atbash_crack_1f84d779}

_____________________________________________________________________________________________________________________________________________________

## ReadMyCert

![image](https://github.com/MeherP2246/PicoCTF_2023_solution/assets/134104519/e0dfd783-5484-4669-8ba8-169737324ba6)

### Solution :

Download the given certificate and open it we will get the flag 

![image](https://github.com/MeherP2246/PicoCTF_2023_solution/assets/134104519/bef351e0-6703-4868-849a-ea78e839927b)

 ### FLag : picoCTF{read_mycert_a7163be8}

_____________________________________________________________________________________________________________________________________________________

## Rotation

![image](https://github.com/MeherP2246/PicoCTF_2023_solution/assets/134104519/c9420947-7f4e-46b8-a674-c103f7646265)

### Solution :

Step 1 : Download the given file and open it it has below content 

xqkwKBN{z0bib1wv_l3kzgxb3l_25l7k61j}

Step 2 : to find the which cipher method it has been used to encode the flag , go to ( ```https://www.dcode.fr/cipher-identifier```) , open the linke and copy paset the data and will get the result as it is encode with ROT Cipher.

Step 3:  Now go to the (```https://www.dcode.fr/rot-cipher```) and copy paste the above cipher and we will get the flag.

 ### FLag : 	picoCTF{r0tat1on_d3crypt3d_25d7c61b}



