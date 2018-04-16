
<b>Help me to become who or what I am!</b><br>

Building the first semantic description of an ethereum-based non-fungible token with JSON-LD and schema.org.<br>

Please, help me to become a valuable member of the semantic web utilizing JSON-LD (1.1) (https://json-ld.org/spec/latest/json-ld/) and the schema.org framework. Hopefully, one day I could become the first non-fungible token with its metadata stored and registered on a cloud registry. I know this exercise could be just a first step. At a certain point in time, of course, my creators (Larva Labs) will have to take over the ownership of my metadata definition, import it into my webpage and maintain it. Please, also do not forget my various interfaces (JSON-RPC (ABI) or other APIs) that could be described here. In the long run this will help the various parties, e.g. Dapp and wallet provider or (rich) snippet designer to have a golden source with standardized metadata.<br>

Please, make sure that the definition passes Google's structured data validator (https://search.google.com/structured-data/testing-tool):<br> https://search.google.com/structured-data/testing-tool?hl=de#url=https%3A%2F%2Fraw.githubusercontent.com%2FCryptopunk3788%2F0xb47e3cd837dDF8e4c57F05d70Ab865de6e193BBB%2Fmaster%2F3788.json

It is fun to find a html JSON-LD header with my metadata like

```
"@context": "http://schema.org",
"@id": "https://myhomepage.com/urn/nft/ethereum-mainnet/0xb47e3cd837dDF8e4c57F05d70Ab865de6e193BBB/3788",
"@type": "VisualArtwork",
"identifier": "urn:nft:ethereum-mainnet:0xb47e3cd837dDF8e4c57F05d70Ab865de6e193BBB:3788",<br>
 ...
 ```

 assuming that my owner (0x1fb9f85fb060c96acb9bd9c38a0586011b34c72d) also owns the myhomepage.com domain


It gets a bit more serious with a JSON-LD header like 

```
"@context": "http://schema.org",
"@id": "https://larvalabs.com/urn/nft/ethereum-mainnet/0xb47e3cd837dDF8e4c57F05d70Ab865de6e193BBB/3788",
"@type": "VisualArtwork",
"identifier": "urn:nft:ethereum-mainnet:0xb47e3cd837dDF8e4c57F05d70Ab865de6e193BBB:3788",
...
```

if my creator (0xc352b534e8b987e036a93539fd6897f53488e56a) owns the larvalabs.com domain


But what about

```
"@context": "http://schema.org",
"@id": "https://explorer.chronicled.org/urn/nft/ethereum-mainnet/0xb47e3cd837dDF8e4c57F05d70Ab865de6e193BBB/3788",
"@type": "VisualArtwork",
"identifier": "urn:nft:ethereum-mainnet:0xb47e3cd837dDF8e4c57F05d70Ab865de6e193BBB:3788",
...
```
         
if a potential registrar(e.g. 0x754c50465885F1Ed1fA1A55b95EE8eCF3f1F4324) owns the <a href="http://explorer.chronicled.org"> explorer.chronicled.org</a> domain, has deployed my contract as well as the <a href="https://github.com/chronicled/open-registry-ethereum">registration contract</a> that my KYC'ed creator(registrant) has used to register me.
