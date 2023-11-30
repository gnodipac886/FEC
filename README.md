# FEC
FEC Codec IP core library for some famous codes (BCH, RS, LDPC, Turbo, Polar and etc)

FEC IP cores are synthesable and self-documented RTL code (System Verilog) with limited functionality and performance to explore or using for any applications. 

The library contain: 
1. BCH code with optional erasures
2. RS code with optional erasures 
3. Viterby code for soft-decoding
4. DVB/Wimax RSC duo-binary turbo code 
5. NASA GSFC LDPC code
6. Wimax LDPC code 
7. 3GPP LDPC code 
8. 3GPP Polar code 
9. Soft decision Golay code 
10. DVB-S2/S2X LDPC code
11. CCSDS Turbo code 
12. 4D-8PSK TCM code 
13. Hamming code 
14. QAM LLR demappers 
15. DVB-S2 PLS code 
16. DVB-S2/S2X BCH code 
17. Wimax BTC (TPC) turbo code

All FEC IP Cores has static configuration and constrained performance. Call me if you need any IP core extension 

# cs229r_project

## Harvard CS229R Project

Code source: [link](https://github.com/dshekhalev/FEC)

| Code        | n, k, d, q        | MAX CLK FPGA | PATH		    						 	| LUT 		  | FF 		    |
| ----------- | -----------    | -----------  | ----------- 							 	| ----------- | ----------- |
| BCH      	  | 255, 223, 4/9, 2  | 438.6 MHz    | berlekamp gamma reg to sigma reg      		| 576         | 315         |
| BCH      	  | 1000, 980, 3/10, 2| 415.5 MHz    | berlekamp gamma reg to sigma reg      		| 825         | 381         |
| LDPC     	  | 576, 480, ???, 2  | 516.8 MHz    | engine llra vn_reg			           		| 4728        | 7869        |
| LDPC     	  | 1056, 880, ???, 2 | 517.1 MHz    | engine llra vn_reg			           		| 4235        | 7674        |
| Hamming  	  | 511, 502, 3, 2    | 204.4 MHz    | data reg to data buffer reg			   		| 991         | 1029        |
| Hamming  	  | 1023, 1014, 3, 2  | 181.3 MHz     | data reg to data buffer reg			   		| 1899        | 2053        |
| RS    	  | 127, 118, 10, 256 | 390.2 MHz    | berlekamp tetta to gamma reg
