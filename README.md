# Algorand .NET Core SDK Blazor Web Application Sample

This is a sample Blazor web application using the Microsoft .NET Core 3.0 Framework and the Algorand SDK. 

All project pages accept inputs of Algorand Node Address and API Token. This example uses a sample Node and API Token provided by Algorand as a developer playground. For information about running your own Algorand Node, please visit https://developer.algorand.org/docs/run-a-node/setup/types/ 

Main project examples are distributed into:
1. Create Address 
  -> used to generate a new Algorand Address and Secret Phrase
  -> No input variables.
  -> Output: Algorand.Account
2. Address Details 
  -> used to view information on specific address
  -> Input: Algorand.Account Secret Phrase
  -> Output: Algorand.Algod.Client.Model.Account 
3. Send Algo 
  -> used to send Algos from a source address to a destination address
  -> Input: Algorand.Account Secret Phrase, Algorand.Address Destination Address, Amount of Algo, Optional Note
  -> Output: Algorand.Transaction 
4. Digital Tokens 
  -> used as landing for all Token based functionality 
4.1. Create New Token
  -> used to create a new Algorand token
  -> Input: Algorand.Account Secret Phrase, Token Name, Unit Name, Default Frozen, Total Amount of Tokens, Token URL, Optional Note
  -> Output: Algorand.Algod.Client.Model.Transaction, Asset ID
4.2. White List Address To Accept Your Token
  -> used to opt address into receiving given token
  -> Input:  Algorand.Account Secret Phrase, Asset ID, Optional Note
  -> Output: Algorand.Algod.Client.Model.Transaction
4.3. Freeze Address To Stop Accepting Your Token
  -> used to opt address out of receiving given token
  -> Input: Algorand.Account Secret Phrase, Algorand.Address Address to Freeze, Asset ID, Optional Note
  -> Output: Algorand.Algod.Client.Model.Transaction
4.4. Destroy Your Token
  -> used to destroy your Algorand token
  -> Input: Algorand.Account Secret Phrase, Asset ID, Optional Note
  -> Output: Algorand.Algod.Client.Model.Transaction
4.5. Use Logic Signature With Your Token
  -> used to 
  -> Input: Algorand.Account Secret Phrase, Asset ID, Program logic to validate, Optional Note
  -> Output: Algorand.Algod.Client.Model.Transaction
5. Send Tokens
  -> used to send your Algorand Token to a white-listed Algorand Address
  -> Input: Algorand.Account Secret Phrase, Algorand.Address Destination Address, Asset ID, Amount of Algo, Optional Note
  -> Output: Algorand.Algod.Client.Model.Transaction
6. Bid Token
  -> used to 
  -> Input: Algorand.Account Secret Phrase, Algorand.Address Address to Auction, Bid Currency, Max Price, Bid ID, Auction ID
  -> Output: Algorand.Transaction, Algorand.Bid
  
Future enhanements include...
  
