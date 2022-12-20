## Squashed Hack The Box walkthrough

Squashed by https://twitter.com/sayli_ambure

Link: https://www.hackthebox.com/machines/squashed


## Solution

#### 1. Sudo nmap -sC -sV -T4 squashed.htb

![](Assets/1.png)

#### 2. showmount -e squashed.htb

![](Assets/2.png)

#### 3. check folder owner's userid

![](Assets/3.png)

#### 4. Add new user with user id 2017 

![](Assets/4.png)

#### 5. Check folder content

![](Assets/5.png)

#### 6. Change user to xx and check folder content

![](Assets/6.png)

#### 7. Copy reverse shell to folder

![](Assets/7.png)

#### 8. Use netcat on 1234 in terminal 2 and open curl http://10.10.11.191/shell.php in terminal 1 

![](Assets/8.png)


#### 9. user.txt has the user flag

![](Assets/9.png)

#### 10. Add new user with user id 1001

![](Assets/10.png)

#### 11. Copy .Xauthority's base64 code

![](Assets/11.png)

#### 12. Decode it and save it in shell > export > take a screenshot

![](Assets/12.png)

#### 13. Start python server in tmp

![](Assets/13.png)

#### 14. Download it in our machine and convert to .png

![](Assets/14.png)

#### 15. Open it and you can see the root password

![](Assets/15.png)

#### 16. Use the password for ssh and the root flag in root.txt

![](Assets/16.png)
