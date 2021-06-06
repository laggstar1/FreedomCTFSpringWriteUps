# Discord 1

Website: [FreedomCTF](https://freedomctf.org/)

---

## Category: Miscellaneous

## Rank: Rare

## Hint: For arguments with more than one word, put them in "" (after &&discordr).

## Question: There seems to be a role that will allow you to find a flag. Use the "&&discordr" to get started!

---

## Website

### Steps to get the flag:
* Steps:
    * *&&discordr role* which returns: "Didn't you learn your lesson from last time! hint: &&flag"
    * *&&flag* which returns: "You are so rude!! No flag for you..."
    * *&&flag please* which returns: "You are nice I will give you something but don't expect a lot! If you treat me well you will be rewarded. Keep that in mind"
    * *&&discordr "role please"* which returns: "6f6e6c792062696e617279"
    * *convert 6f6e6c792062696e617279 from hex to plain text to get "only binary"*
    * *convert "only binary" to binary to get "01101111 01101110 01101100 01111001 00100000 01100010 01101001 01101110 01100001 01110010 01111001"*
    * *&&discordr "01101111 01101110 01101100 01111001 00100000 01100010 01101001 01101110 01100001 01110010 01111001"* which adds "role seeds.length()" role to your roles"
    * *Then you can look in the "role-lenseeds" channel where the flag is listed: "flag{see|)s_aRe_n0t_so_raNdom?}"*