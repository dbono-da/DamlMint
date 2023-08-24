# DamlMint

This application allows a Minter to create a mint and generate tokens that can be owned by other parties

### TO NOTE:
The minter by design has to authorize transfers of tokens. This is because without this, anyone could just "Create" a counterfeit token contract and list the minter as a valid mint. Adding the minter as a signatory on the token prevents _anyone_ from creating a token contract and listing _anyone_ as the mint. This has the side effect though of requiring the token to be created again when the transfer happens. There for sure are better ways to deal with this paradigm, but this repo was just created for the daml fundamentals cert, to demonstrate daml basics. 


# Running

This application can be run with `daml start` and the navigator can be used to interact with contracts created by the involved parties 


# Basic Workflow

1. Create Mint
2. Mint a token w/ minter as owner
3. Propose Transfer to another party
4. Party Accepts the transfer
5. Recipient confirms the transfer 

# Basic continuing workflow
1. Token Holder proposes a transfer
2. New holder approves tansfer
3. Token holder and the mint confirm the transfer (the mint confirms it to make sure that the token is not a counterfit)


