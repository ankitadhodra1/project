# NFT Metadata Collector

This is a simple JavaScript project designed to mint NFTs (Non-Fungible Tokens), store their metadata, list all the minted NFTs, and get the total supply of NFTs created.


## Description
This program is in JavaScript , In this users can create new NFTs by specifying metadata attributes such as name, eye color, shirt type, and bling.
## Getting Started
## Executing Program
To run this program, you can use Gitpod https://gitpod.io/#https://github.com/MetacrafterChris/Beginning-Javascript

Once you are on the Gitpod website, create a new file . Save the file with a ".js" extension (e.g. project.js). Copy and paste the following code into the file:




bash
            
             
             /*
                Assessment Requirements
         1. Create a variable that can hold a number of NFT's. What type of variable might this be?
         2. Create an object inside your mintNFT function that will hold the metadata for your NFTs. 
         The metadata values will be passed to the function as parameters. When the NFT is ready, 
         you will store it in the variable you created in step 1
        3. Your listNFTs() function will print all of your NFTs metadata to the console (i.e. console.log("Name: " + someNFT.name))
        4. For good measure, getTotalSupply() should return the number of NFT's you have created
        */

        // create a variable to hold your NFT's
      const NFTs = []

      // this function will take in some values as parameters, create an
      // NFT object using the parameters passed to it for its metadata, 
      // and store it in the variable above.
      function mintNFT (_name,_eyeColor,_shirtType,_bling) {
        const NFT = {
     "name":_name,
     "eyeColor":_eyeColor,
     "shirtType":_shirtType,
     "bling":_bling
      }
      NFTs.push(NFT);
      console.log("Minted:"+ _name);
      }

      // create a "loop" that will go through an "array" of NFT's
      // and print their metadata with console.log()
      function listNFTs () {
      for(let i=0; i<NFTs.length; i++){
     console.log(NFTs[i]);   
      }
      }

      // print the total number of NFTs we have minted to the console
      function getTotalSupply() {
    console.log(NFTs.length);
    }

    // call your functions below this line
    mintNFT("Ankita","Black","Beige","Chain");
    listNFTs();
      getTotalSupply(); 

In this code

Mint NFTs: Users can create new NFTs by specifying metadata attributes such as name, eye color, shirt type, and bling.

Store Metadata: The project maintains an array to store metadata for each minted NFT.

List NFTs: Users can view a list of all NFTs along with their associated metadata.

Total Supply: Users can determine the total number of NFTs created.

than compile and run this code will be executed.






## Author

- ANKITA
  ankita756900@gmail.com



## License

This project is licensed under [MIT](https://choosealicense.com/licenses/mit/) License - see the LICENSE.md file for details
