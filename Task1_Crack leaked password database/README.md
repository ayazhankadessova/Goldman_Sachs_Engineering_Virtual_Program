# Goldman-Sachs-Crack-Leaked-Passsword-Database
## Password Controls and Security Policies

### Overview 
As a governance analyst it is part of your duties to assess the level of protection offered by implemented controls and minimize the probability of a successful breach. You often need to know the techniques used by hackers to circumvent implemented controls and propose uplifts to increase the overall level of security in an organization. Gaining valid credentials gives the attackers access to the organization’s IT system, thus circumventing most of perimeter controls in place.

## Project Objectuve
`What type of hashing algorithm was used to protect passwords?`

`What level of protection does the mechanism offer for passwords?`

`What controls could be implemented to make cracking much harder for the hacker in the event of a password database leaking again?`

Here is a sample data file containing hashes dumped together:

Leaked passwords - passwords that have been gained by the attackers.

After analysing the hashed:

1. The organization uses an outdated password hashing algorithm (MD5). It offers very little protection because it can be easily replicated.

2.  Thepassword policy the organization has is not aligned with modern safer pratices. It allows users have short passwords (6 characters) and reuse usernames as in the passwords. 

Not to let attackers gain access to the organization’s IT system, thus circumventing most of perimeter controls in place the organization is advised to:

•	Use a better password hashing algorithm. Examples: bcrypt, scrypt or PBKDF2. This will greatly increase the time needed to crack individual passwords, to years!

•	Implement salting to prevent usage of rainbow tables to speed up cracking,

•	Increase the minimum password length requirement to 10 characters at least. Long passwords require greated computational effort required to crack & will give additional time to change all passwords in the event of the password database being leaked,

•	Prevent passwords to be the same as usernames or reused as part of the password – such password combination is easy to check without gaining access to the password database itself.  

•	It is advised to educate users on creating safe and easy to remember passwords, such as advise using special characters and numbers as easy to remember substitutions to expand the key space (e.g. mYgranny$cha1rhadstaples)

•	Educate users on the benefits of passwords managers. They can have random, but long passwords that way s (e.g. M>?{tk6Cfep6BrZ4J)KZWQ8j) without the need to remember/write down. A strong passphrase is still required as a master key for to access the password manager.

•  2FA Authentication. If the password is cracked, it is not enough!

# Project Report and Observations 

Exploreing the task and Hashing ALgorithms, MD5 and SHA were the two algorithms that I saw. Analysing the passwords and algorithms, I concluded the following, which are presented in my report.

## Project Report
```
To Whome it may concern,

After trying to crack all the leaked hashes, I found several vulnerabilities in your password policy. Therefore, i have some suggestions to improve your password policy.

Secure Hash Algorithm (SHA) and Message Digest (MD5) are the standard cryptographic hash functions 
to provide data security for authentication. 

I could easily crack most of your passwords using MD5. I am sure I could crack them all given larger wordlist. MD5 is prone to collisions. It was very easy to crack with Hashcat.com and rockyou.txt wordlist via terminal and web browsers & even through my own code!
I would suggest that you use stronger password encryption mechanism to create hashes for the password based on SHA.

Current password policy:
• Minimum length for password is set to 6.
• There is no specific requirement for the password creation. 

My recommendations for the better password policy are:
• Avoid common words and character combinations in your password.
• Longer passwords are better, 8 characters is a starting point.
• Don’t reuse your passwords.
• Include special character, Capital and Small letters, numbers in your password.
• Don’t let users include their username, actual name, date of birth and other personal information while creating a password.
• Train your users to follow these policies to keep their passwords safe.

Thanking you, 
Name: Ayazhan Kadessova

```
## Observations:
```
Leaked passwords: 
experthead:e10adc3949ba59abbe56e057f20f883e
interestec:25f9e794323b453885f5181f1b624d0b
ortspoon:d8578edf8458ce06fbc5bb76a58c5ca4
reallychel:5f4dcc3b5aa765d61d8327deb882cf99
simmson56:96e79218965eb72c92a549dd5a330112
bookma:25d55ad283aa400af464c76d713c07ad
popularkiya7:e99a18c428cb38d5f260853678922e03
eatingcake1994:fcea920f7412b5da7be0cf42b8c93759
heroanhart:7c6a180b36896a0a8c02787eeafb0e4c
edi_tesla89:6c569aabbf7775ef8fc570e228c16b98
liveltekah:3f230640b78d7e71ac5514e57935eb69
blikimore:917eb5e9d6d6bca820922a0c6f7cc28b
johnwick007:f6a0cb102c62879d397b12b62c092c06
flamesbria2001:9b3b269ad0a208090309f091b3aba9db
oranolio:16ced47d3fc931483e24933665cded6d
spuffyffet:1f5c5683982d7c3814d4d9e6d749b21e
moodie:8d763385e0476ae208f21bc63956f748
nabox:defebde7b6ab6f24d5824682a16c3ae4
bandalls:bdda5f03128bcbdfa78d8934529048cf


Cracked Passwords with md5:
hashed_string,password
e10adc3949ba59abbe56e057f20f883e,123456
25f9e794323b453885f5181f1b624d0b,123456789
d8578edf8458ce06fbc5bb76a58c5ca4,qwerty
5f4dcc3b5aa765d61d8327deb882cf99,password
96e79218965eb72c92a549dd5a330112,111111
25d55ad283aa400af464c76d713c07ad,12345678
e99a18c428cb38d5f260853678922e03,abc123
fcea920f7412b5da7be0cf42b8c93759,1234567
7c6a180b36896a0a8c02787eeafb0e4c,password1
6c569aabbf7775ef8fc570e228c16b98,password!
3f230640b78d7e71ac5514e57935eb69,qazxsw
917eb5e9d6d6bca820922a0c6f7cc28b,Pa$$word1
f6a0cb102c62879d397b12b62c092c06,bluered
```
Complete report is available at: 

https://github.com/ne3lakolkar/Goldman-Sachs-Crack-Leaked-Passsword-Database/blob/main/SHA%20Hashes%20and%20Goldman%20Sachs%20Internship.pdf

## Resources 

https://arstechnica.com/information-technology/2013/05/how-crackers-make-minced-meat-out-of-your-passwords/

https://howsecureismypassword.net/

https://en.wikipedia.org/wiki/Password_cracking#Software

https://en.wikipedia.org/wiki/Salt_(cryptography)

https://hashcat.com

https://colab.research.google.com/github/mxrch/penglab/blob/master/penglab.ipynb#scrollTo=vp4LSKizX-8E  , 

https://github.com/mxrch/penglab

https://towardsdev.com/building-a-hash-cracking-tool-using-python-ea15768409ef