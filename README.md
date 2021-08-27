# Air-Master-AM7
This is research of Air Master AM7 USB(Serial) communication protocol.
It was based on desktop application "AirMaster Control Pannel v1.2"

####Upload zip archieve to Google Drive and Share the link below.###

The final goal  is to replace base WiFi module with modificated software some hardware modification (change RX and TX lines).

In the future there are Logic Analyzer logs, photos and additional research information will be added.


Read Data Command
U\xCDG\0\0\0\0\0\0\x01i
85	205	71	0	0	0	0	0	0	1	105	13	10


Response 40 bytes
srvc	20			23	  	0.011		0.222		 556		29.38	 	  54.19					srvc	    2472		  703   	  104	 	 10     	 6							    		srvc	round	rest	\r  \n
170		0	20		0	23		0	11		0	222		2	44		11	122		21	43	   1	4	0	0   	9	168		2	191		0	104		0	10		 0	6  	0	0	0	0	0	0	      71    	4		231		13	10
    PM2.5	  	PM10		HCHO		TVOC		CO2			 TMP			HUM				        	  	 03um		 05um	 	1.0um		2.5um		 5.0um
                                      x2x2C    xBx7A    x15x2B                 x9xA8     x2xBF    
		
Set Date Command
U	  \xCD	E 	\x15	\x04  	\x1E   	  \x07	  7	    \x0F	  \x01	\xEB  \x01  \xF6
85	205		69	21		4		      30	  	7		    55	    15	  	1		235     13    10
              year  month    day      hour  minute  second  rnd   rest    \r    \n
              
Response
\xAA\x01\x01\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\xAC
