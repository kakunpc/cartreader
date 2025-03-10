### Copy these files to the root of your SD card.  

## gba.txt  
This file stores the GBA database which is needed because the save type and rom size are not stored inside the rom. 

Example:  
A22J,08,3   
game id, size in MByte, savetype  

Savetypes:   
0 = Unknown or no save   
1 = 4k Eeprom   
2 = 64K Eeprom   
3 = 256K Sram   
4 = 512K Flash   
5 = 1024K Flash   
6 = 512K Sram   

## n64.txt  
This file stores the N64 database which is needed because the save type and rom size are not stored inside the rom.  
The CRC32 checksum is used to verify a good dump.  

Example:  
002c3b2a,NO7P,32,0  
CRC32, game id, size in MByte, savetype  

Savetypes:  
0 = no save chip  
1 = SRAM  
4 = Flashram  
5 = 4K Eeprom  
6 = 16K Eeprom  

## nes20db.txt  
Database for NES cartridges.     

## PCE_CRC_LIST.txt    
Placing this file into the root of the SD card will enable verify and automatic game name identifier.    

## snes.txt  
This file is needed for odd sized SNES games like Final Fantasy (JAP), Super Metroid(US/JAP) or Tales of Symphonia. Without this file you will get overdumps and the checksum calculation will fail. This list was generated by a simple script and might contain many errors.    

Example:  
A172,24,48  
checksum, size in Mbit, number of banks (lorom needs twice as many banks as hirom for the same rom size, lorom: 32kb banks, hirom: 64kb banks)    

## snes_clk.txt    
Calibration data for clock generator.     
