# Algorand .NET Core SDK Blazor Web Application Sample

This is a sample Blazor web application using the Microsoft .NET Core 3.0 Framework and the Algorand SDK. 

All project pages accept inputs of Algorand Node Address and API Token. This example uses a sample Node and API Token provided by Algorand as a developer playground. For information about running your own Algorand Node, please visit https://developer.algorand.org/docs/run-a-node/setup/types/ 

Main project examples are distributed into:
1. Create Address 
  a) Used to generate a new Algorand Address and Secret Phrase
  b) No input variables.
  c) Output: Algorand.Account
  
2. Address Details 
  a) Used to view information on specific address
  b) Input: Algorand.Account Secret Phrase
  c) Output: Algorand.Algod.Client.Model.Account 
  
3. Send Algo 
  a) used to send Algos from a source address to a destination address
  b) Input: Algorand.Account Secret Phrase, Algorand.Address Destination Address, Amount of Algo, Optional Note
  c) Output: Algorand.Transaction 
  
4. Digital Tokens 
  a) used as landing for all Token based functionality 
  
5. Create New Token
  a) used to create a new Algorand token
  b) Input: Algorand.Account Secret Phrase, Token Name, Unit Name, Default Frozen, Amount of Tokens, Token URL, Optional Note
  c) Output: Algorand.Algod.Client.Model.Transaction, Asset ID
  
6. White List Address To Accept Your Token
  a) used to opt address into receiving given token
  b) Input:  Algorand.Account Secret Phrase, Asset ID, Optional Note
  c) Output: Algorand.Algod.Client.Model.Transaction
  
7. Freeze Address To Stop Accepting Your Token
  a) used to opt address out of receiving given token
  b) Input: Algorand.Account Secret Phrase, Algorand.Address Address to Freeze, Asset ID, Optional Note
  c) Output: Algorand.Algod.Client.Model.Transaction
  
8. Destroy Your Token
  a) used to destroy your Algorand token
  b) Input: Algorand.Account Secret Phrase, Asset ID, Optional Note
  c) Output: Algorand.Algod.Client.Model.Transaction
  
9. Use Logic Signature With Your Token
  a) used to 
  b) Input: Algorand.Account Secret Phrase, Asset ID, Program logic to validate, Optional Note
  c) Output: Algorand.Algod.Client.Model.Transaction
  
10. Send Tokens
  a) used to send your Algorand Token to a white-listed Algorand Address
  b) Input: Algorand.Account Secret Phrase, Algorand.Address Destination Address, Asset ID, Amount of Algo, Optional Note
  c) Output: Algorand.Algod.Client.Model.Transaction
  
11. Bid Token
  a) used to 
  b) Input: Algorand.Account Secret Phrase, Algorand.Address Address to Auction, Bid Currency, Max Price, Bid ID, Auction ID
  c) Output: Algorand.Transaction, Algorand.Bid
  
Future enhanements include...
  
