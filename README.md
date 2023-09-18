# Performing Search for Sensitive Data Exposure .GIT & Decrypt Password

We are going to search any sensitive data .git hidden files using dirsearch and limit the search by -x 300-600.\
-u for our target url
-x for limit the search

![1](https://github.com/ggouw/Sensitive-Data-Exposure-GIT/assets/120260071/9ea4805f-80c9-4f42-b31b-35677482d02d)

Use "ls' to check what folder we have, use "cd" to access the folder and "tree" for folder structure.

![2](https://github.com/ggouw/Sensitive-Data-Exposure-GIT/assets/120260071/5f9f66f2-3425-4858-a99a-751b9434acdb)\
![3](https://github.com/ggouw/Sensitive-Data-Exposure-GIT/assets/120260071/ad48e102-83c3-4f16-ba22-3c10187bcb19)

Download file from .git using 'gitdumper'.

![4](https://github.com/ggouw/Sensitive-Data-Exposure-GIT/assets/120260071/9027fbee-4455-4ef2-8c82-5917b7056065)\
![5](https://github.com/ggouw/Sensitive-Data-Exposure-GIT/assets/120260071/b0200211-b910-46d3-b591-823e5008e978)

Check the result in Gittools - Extractor folder.

![6](https://github.com/ggouw/Sensitive-Data-Exposure-GIT/assets/120260071/9b0d1ead-fee0-4ce8-ac12-2d93f08ad067)

We found user_message_database.sql in this folder.

![7](https://github.com/ggouw/Sensitive-Data-Exposure-GIT/assets/120260071/4fc8a749-7ea7-4269-af62-aef76232d134)

if we open the folder user_message_database.sql, no important files save in this folder.

![8](https://github.com/ggouw/Sensitive-Data-Exposure-GIT/assets/120260071/bb7cb073-2c90-47e9-9aa1-ede5238f6159)

But in the beginning when we ran dirsearch to our url target, we have found db.sql file.

![10](https://github.com/ggouw/Sensitive-Data-Exposure-GIT/assets/120260071/85feab6d-5572-46a1-b435-d7fa5b2b39f9)

The next step for this is to try open the url in our browser\
https://localhost:2222/dirsearch/db.sql

![13](https://github.com/ggouw/Sensitive-Data-Exposure-GIT-and-Decrypt-Password/assets/120260071/e2e6b0f1-cae1-40e5-8022-1cda3c23bf7b)\
![14](https://github.com/ggouw/Sensitive-Data-Exposure-GIT-and-Decrypt-Password/assets/120260071/33fb30ae-0710-4788-811a-b2c263aef24c)

Then we found the list of username and password.

![15](https://github.com/ggouw/Sensitive-Data-Exposure-GIT-and-Decrypt-Password/assets/120260071/b8475b0d-5149-405a-a143-d2ac6ac849a7)

After this we can use Has Analyzer to examine what type of data is this.

![16](https://github.com/ggouw/Sensitive-Data-Exposure-GIT-and-Decrypt-Password/assets/120260071/ed6d46cf-d107-428f-a267-3115c4dee604)

From here, we know that this is MD5 or MD4 type of data. We can use MD5 decrypt tools to decrypt the password.

![17](https://github.com/ggouw/Sensitive-Data-Exposure-GIT-and-Decrypt-Password/assets/120260071/7bcf64d2-9f60-40cd-bdd2-ec838e72cc4f)

After decrypt, We found Password for Username rivera92 is 791164.




















