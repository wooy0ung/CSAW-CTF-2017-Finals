CHAL NAME: ethersplay
AUTHOR: quend

POINTS: 400 (we can raise it if no one solves it the first day)

CATEGORY: RE

DESC FOR LEADERBOARD:
I stole this contract from a private blockchain. Can you help me reverse its secrets?

FLAG:
flag{ETHBTC_tothemoon}

Distribute .abi and .bytecode files.

JUDGE DESC (solution walkthrough):
Its solidity bytecode. So players must:
1) figure out how to reverse it (the name of the challenge is a hint to tooling)
2) figure out which function is a good target function - aka which has 'flag' in it
3) find the winning path in the function - when you pass in the right username it will print out something different
4) figure out what algo is used to hash the password (its SHA1)
5) recover the flag through brute forcing 6 characters in SHA1
6) submit the flag 
