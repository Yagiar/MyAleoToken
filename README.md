# token_1693.aleo

## Code Overview:

The Aleo program defines a simple token system with two main structs: Token and token_1693.

`struct Token`: Represents a token with two fields, `owner` (an address) and `balance` (an unsigned 32-bit integer).
`transition mint`: Allows minting new tokens with a specified balance and assigns the caller as the owner.
`transition transfer`: Allows transferring tokens from the caller to another address, updating both the recipient's and sender's token balances.

## Mint

In the `.env` file, specify your private key for your token deployment to work correctly.
Now in the file `token_1693.in` on the function `mint` change the value for the number of tokens minting (in the program 100).

Now you can run:
```bash
leo run mint
```
As a result, we have a record of the output of the `mint` function.

## Transfer 
Now take the output data obtained as a result of the `mint` function.
Insert it into the `.env` file in the `transfer` function section without `private` and `public` suffixes.
Also don't forget to replace the recipient and the number of tokens to be transferred.

And run:
```bash
leo run transfer
```

Discord: Attak Helicopter#9164
