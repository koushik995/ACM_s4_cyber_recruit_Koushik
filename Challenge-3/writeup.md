# Challenge Description

I got the letter from hogwarts but it was password encrypted help me to find, lets try until we get the password the password for the pdf. In that pdf u can get the flag.

---

# Analysis and Approach

The PDF could not be opened. It required a password. So, it’s about password cracking. And in image it is said that "no muggle should read it".There was no visible hint inside the PDF name itself. So the password had to be extracted.

I suspected it is likely in a wordlist.
I used pdfinfo to get the type of pdf and returned an error saying the password was incorrect, confirming encryption.I also checked encryption type using qpdf, it is standard encrypted pdf

To crack the password, I needed to extract the hash in a format compatible with cracking tools. Using John(pdf2john). After extracting the hash, we get $pdf$ formatted hash, which confirmed successful extraction.

I first used rockyou wordlist. Since it was compressed, I decompressed it using gunzip. Then i ran John with the wordlist, John tested all passwords from the list, it successfully cracked password. then by showing the password "bud121clam725"

Using the cracked password bud121clam725, I opened the PDF file successfully.
Inside the document, I found the hidden flag.

---

# Tools / Commands Used

- pdfinfo
- qpdf
- rockyou.txt
- john
- wordlists
- gunzip
- pdf2john
- pdfcrack 

---

# Final Flag

potter{w3lc0m3_70_h0gw4r75}
