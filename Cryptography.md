# HideToSee

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





