 #Disclaimer: I didn't slove this Challenge during the CTF is live. But i am so close to solve. So i write this Writeup.

Challenge_Name: Null Food Factory. Description: Prove your hacking skill to get admin panel. Author: r3curs1v3_pr0xy

# Sql (not worked at all)
i tried all the payload. But not work.

# Try to identify what attack (get help)
I saw the (interesting message) in (GrabCon_CTF) discord chat.
It was ("When i excute the %00, It was output some crazy codes"). 
So i knew that it can be (null byte injection).  (I Stopped on this when the CTF is really live. Because I Didn't get much time to find good resources during the ctf is live. 
So that i can't solved the challenge.)

# Finding_Resources
https://www.whitehatsec.com/glossary/content/null-byte-injection

# Note_For_Solution
We can register the account. So we can excute the our injection in register input box.
And Remember the (Description). We only need to get admin account.

# Final_Solution
We can fill anything in (first name and last name).
We will put our (injection code) in (Username form). Payload = "admin%00"
And we can set anything in (password Form). And When we register, The Website Return the text 
"Admin Password Has been updated to ic8aGsk^bh"
So now we can login as (admin). 
Username = admin and Password = ic8aGsk^bh. When we login, We got flag.

# Flag: GrabCON{Null_byt3s_1s_L0v3}

# #Disclaimer: I didn't slove this Challenge during the CTF is live. But i am so close to solve that Challenge. So i write this Writeup.
