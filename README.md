# QRcryptor
QR encrypted data generator


# Files
  QRnumberGen: generates and encrypts numbers in a range from 0 to 1000 (usually for lottery tickets to prevent forgery) and then
    generates QR codes with each crypted number and saves them
  * Modules used: qrcode, cryptography, PIL
    
  QRdecryptor: decrypts QR crypted texts with given key, .exe file created with auto-py-to-exe, it also contains some garnish
     in order for the .exe file look better
  * Modules used: Cryptography, time, random, tqdm, pyfiglet, keyboard, os, termcolor, pynput
        
# Program details
   Mainly dedicated to Oviedo university to help and prevent forgery in lottery tickets. 
   Actually being used as a security system for a raffle going on. No issues found yet.
   
# Program features
   * Mainly focused on number encryption to avoid forgery
   * Opens file key.key with stored fernet key to encrypt numbers
   * Generate numbers in a custom range
   * Encrypts numbers with cryptography module using Fernet with a simple randomly generated key.
   * Converts the previosuly generated and encrypted numbers into QR codes (Usually for pasting them in any kind of protected document)
   * Saving QR codes with format 'No{n}.png' being n the crypted number
   
   QRdecryptor: 
   * Decrypts QR codes using Fernet (cryptography module) and the previosuly used key to generate encrypted numbers.
   
   
   
      
  
