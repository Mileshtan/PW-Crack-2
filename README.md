# PW-Crack-2
Cylab CTF PW Crack 2

Q: Can you crack the password to get the flag? Download the password checker here https://challenge-files.cylabacademy.net/library/227623e9501e3a811cdf5b1c7a2079f75b2e9ab243364a38830e0a4a2943ce2e/level2.py
 and you'll need the encrypted flag https://challenge-files.cylabacademy.net/library/227623e9501e3a811cdf5b1c7a2079f75b2e9ab243364a38830e0a4a2943ce2e/level2.flag.txt.enc
 in the same directory too.

 Hint1: Does that encoding look familiar?

 Hint2: The str_xor function does not need to be reverse engineered for this challenge.

 Step1: Download both the file  level2.py and level2.flag.txt.enc
 wget https://challenge-files.cylabacademy.net/library/227623e9501e3a811cdf5b1c7a2079f75b2e9ab243364a38830e0a4a2943ce2e/level2.py
 wget https://challenge-files.cylabacademy.net/library/227623e9501e3a811cdf5b1c7a2079f75b2e9ab243364a38830e0a4a2943ce2e/level2.flag.txt.enc

 Step2: cat level2.py and copy chr(0x34) + chr(0x65) + chr(0x63) + chr(0x39)

 Step3: python3
 and paste chr(0x34) + chr(0x65) + chr(0x63) + chr(0x39)
 and output is 4ec9

 Step4: python3 level2.py
 type password 4ec9

<img width="537" height="477" alt="image" src="https://github.com/user-attachments/assets/d1f15061-3879-45eb-97ed-b2307aa445ad" />

 Step5: Final Answer: academy{tr45h_51ng1ng_d99a9ef4}
