# Cookies-Writeup-picoCTF

**Description:**

Who doesn't love cookies? Try to figure out the best one. http://mercury.picoctf.net:21485/

**SOLUTION**

1. Go to the website

2. If you play around with the site you'll notice that if you enter certain cookie names, you'll be taken to a page that says "I love <cookie name entered>"

3. If you enter something different then you'll get an invalid input error

4. Inspect the element of the site and go to the **STORAGE** tab

5. You'll notice how you can actually change the value of the cookie. If you change the value, refresh the page, you'll get a different cookie name **THIS IS IMPORTANT**

6. You can manually dig through each value and find the flag, but what if the website contians 1,000 values?

7. Write a Python program that runs through the values and stop when it finds something that doesn't contain "I love"

If you're not proficient in Python, feel free to use my cookie.py file
