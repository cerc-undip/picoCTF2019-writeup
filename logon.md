# LOGON

The factory is hiding things from all of its users. Can you login as logon and find what they've been looking at? `https://2019shell1.picoctf.com/problem/47307/` ([link](https://2019shell1.picoctf.com/problem/47307/)) or http://2019shell1.picoctf.com:47307
## SOLUTION

 

 - By opening the link given you are redirected to a website which require login credentials.
 - Enter any Username and Password
 - Now Use inspect element feature in your browser and go to storage section
 - There you can see the username and password you entered and admin cookie.
 ![alt text](https://user-images.githubusercontent.com/44405294/66729496-709fac00-ee69-11e9-8133-d6c8dfdbabf1.png)
 - Change value of admin from **False** to **True**
 
 **Flag**:
 ![alt text](https://user-images.githubusercontent.com/44405294/66729500-74333300-ee69-11e9-930e-291c308960df.png)

