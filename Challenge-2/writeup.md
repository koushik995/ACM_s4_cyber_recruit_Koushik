# Challenge Description

I found the this wand. I don’t know whose wand is so i need to find it and also the flag is inside this image. Go on, you may find the hint.

---

# Analysis and Approach

The file had no extension.The file type is probably being disguised intentionally.It’s either contains embedded data or hiding something inside another file.

So,I suspected that It could be an image with hidden data or could contain appended data or might contain readable strings.

I tried strings, file, exiftool commands on the given wand.jpeg file, there i found the metadata and re-Confirmed it with other mentioned commands, i.e Comment: password: "Full name of the weilder without spaces in small letters"

Name of the weilder is Albus Dumbledore, his full name without spaces in small letters is "albuspercivalwulfricbriandumbledore". So, then using steghide, it asks passphrase which was albuspercivalwulfricbriandumbledore, then an embedded file hide.txt shows up, it contains the flag.

---

# Tools / Commands Used

- strings
- file
- exiftool
- steghide

---

# Final Flag

potter{1_570l3_7h47_3ld3r_w4nd}
