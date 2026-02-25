# Challenge Description

Someone from the Hogwarts send this file given below to the voldemort.I don’t know who it is and what is the information in it. What ever the information is but it will definitely harm harry so find the person who send it. The flag lies there. Author: murder

---

# Analysis and Approach

We were given an image file named “top secret.png”. The name itself suggested that something was hidden inside the image and it is containing other person talking sarcasticly with voldemort. and a reciever.txt file : "This message is sent to voldemort, No muggle should read it"

I thought of steganography and ran binwalk,exiftool,steghide and got error and renamed it without space.

I first checked the metadata using exiftool, nothing is unusual.Next, I used binwalk, i couldnt find any data, then Since it was a PNG file and involved steganography, I tried steghide and passphrase is "why always my nose",it leads to access (secret,important.txt) files, horrcrux.jpg is .secret directory, it is extracted and got "cG90dGVyezdoMTVfMTVfRDAxMHIzNV9VbThyMWRnM30=", it led to the flag using base64.

---

# Tools / Commands Used

- binwalk
- exiftool
- steghide
- find

---

# Final Flag

potter{7h15_15_D010r35_Um8r1dg3}
