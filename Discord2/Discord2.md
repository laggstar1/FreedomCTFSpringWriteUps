# Discord 2

Website: [FreedomCTF](https://freedomctf.org/)

---

## Category: Miscellaneous

## Rank: Rare

## Hint: For arguments with more than one word, put them in "" (after &&assignrole).

## Question: There seems to be a role that will allow you to find a flag. Use the "&&assignrole" to get started!

---

## Website

* Steps to get the flag:
    * *&&flag* which returns: "You are so rude!! No flag for you..."
    * *&&flag "pretty please"* which returns: "You want the flg? Here is something that might help. https://pastebin.com/QbFAJK4p"
    * *From the link you see an assign_role() function, so call assign_role()*
    * *&&assignrole* which returns: "&&assignrole <arg>"
    * *&&assignrole 1* which returns: "No roles for you! 😝"
    * *You will want to brute force this and when you do "&&assignrole 15" you will get a direct message saying: Might want to check your roles? 😉"
    * *When you check your role list, you will see a role named, "Flag Receivers" and will have access to a hidden text channel named, "flags". In there is the flag, "flag{s33ds_4re_FuN!}."*