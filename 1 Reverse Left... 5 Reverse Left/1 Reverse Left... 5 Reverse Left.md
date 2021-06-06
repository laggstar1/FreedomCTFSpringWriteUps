# 1 Reverse Left... 5 Reverse Left

Website: [FreedomCTF](https://freedomctf.org/)

---

## Category: Cryptography

## Rank: Epic

## Hint: Remove "X" after if there are any leftovers at the end of every line after a reverse.

## Question: My math teacher sent this to me saying they wanted to show this to the class, but wanted to test this out with me first. Can you find out what it says?

    Message: ct1a0aF_i_nrbut1t0ryX_XXXXXX1X

---

## Website

### Looking at the title, you see "1 Reverse Left... 5 Reverse Left", from that you should seperate the phrase into spaces starting from 1 and reverse the characters, and keep on repeating this until you get it seperated into 5 characters per space:

<br></br>
//Initial

### ct1a0aF_i_nrbut1t0ryX_XXXXXX1X

//Seperate into 1

c t 1 a 0 a F _ i _ n r b u t 1 t 0 r y X _ X X X X X X 1 X

//Reverse

c t 1 a 0 a F _ i _ n r b u t 1 t 0 r y X _ X X X X X X 1 X

---

//Seperate into 2

ct 1a 0a F_ i_ nr bu t1 t0 ry X_ XX XX XX 1X

//Reverse

tc a1 a0 _F _i rn ub 1t 0t yr _X XX XX XX X1

---

//Seperate into 3

tca 1a0 _F_ irn ub1 t0t yr_ XXX XXX XX1

//Reverse and remove the two X after the "1" at the end

act 0a1 _F_ nri 1bu t0t _ry XXX XXX 1XX

---

//Seperate into 4

act0 a1_F _nri 1but 0t_r yXXX XXX1

//Reverse and remove three X after the "1" at the end

0tca F_1a irn_ tub1 r_t0 XXXy 1XXX

---

//Seperate into 5

0tcaF _1air n_tub 1r_t0 XXXy1

//Reverse and remove the three X after the "y" at the end

Fact0 ria1_ but_n 0t_r1 1yXXX

---

//flag:

### Fact0ria1_but_n0t_r11y



<br></br>
<br></br>
<br></br>
<br></br>

Fact0ria1_but_n0t_r11y

Fact0 ria1_ but_n 0t_r1 1yXXX

0tcaF _1air n_tub 1r_t0 XXXy1

0tca F_1a irn_ tub1 r_t0 XXXy 1XXX

act0 a1_F _nri 1but 0t_r yXXX XXX1

act 0a1 _F_ nri 1bu t0t _ry XXX XXX 1XX

tca 1a0 _F_ irn ub1 t0t yr_ XXX XXX XX1

tc a1 a0 _F _i rn ub 1t 0t yr _X XX XX XX X1

ct 1a 0a F_ i_ nr bu t1 t0 ry X_ XX XX XX 1X

c t 1 a 0 a F _ i _ n r b u t 1 t 0 r y X _ X X X X X X 1 X

c t 1 a 0 a F _ i _ n r b u t 1 t 0 r y X _ X X X X X X 1 X

ct1a0aF_i_nrbut1t0ryX_XXXXXX1X