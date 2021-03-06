#CalkaBot 2
C PORT pinout:

| **PORT**|**Function**    			   | **Code** | **Pin** |
|:-------:|:----------------------:|:--------:|:-------:|
| **PB**  | **-** 		   			     |  **-**   | **-**   |
|	PB0     | *empty*		   			     |    -     |   8	 	  |
|	PB1     |	ICSP - SCK	   			   |	-	      |   9     |
|	PB2     |	ICSP - MOSI	   			   |	-	      |   10    |
|	PB3     |	ICSP - MISO	   			   |	-	      |   11    |
|	PB4     |	Motor A control 		   |  `Ma2`   |   28    |
|	PB5     |	Motor A control  		   |  `Ma1`   |   29    |
|	PB6     |	Motor B Control 		   |  `Mb1`	  |   30    |
|	PB7     |	*empty*	   	   			   |	-	      |   12    |
| **PC**  | **-** 		   			     |  **-**   | **-**   |
|	PC6     | Motor B Control 		   |  `Mb2`	  |   31    |
|	PC7     | Motor B PWM    			   |  `MbPWM` |   32    |
| **PD**  | **-** 		   			     |  **-**   | **-**   |
|   PD0   | Right A floor sensor 	 |  `FaR`	  |   18	  |
|   PD1   | Left A floor sensor    |  `FaL`	  |   19	  |
|   PD2   | Left B floor sensor 	 |  `FbL`	  |   20	  |
|   PD3   | Right B floor sensor 	 |  `FbR`	  |   21	  |
|   PD4   | Center B distans sensor|  `IRb`	  |   25	  |
|   PD5   | Right B distans sensor |  `IRbR`  |   22	  |
|   PD6   | Left B distans sensor  |  `IRbL`  |   16	  |
|   PD7   | Motor A PWM    			   |  `MaPWM` |   27	  |
| **PF**  | **-** 		   			     |  **-**   | **-**   |
| 	PF0   | Button 2       		     |  `but3`  |   41    |
| 	PF1   | Button 3       			   |  `but2`  |   40    |
| 	PF4   | Button 4       			   |  `but1`  |   39    |
| 	PF5   | Right A distans sensor |  `IRaR`  |   38    |
| 	PF6   | Center A distans sensor|  `IRa`	  |   37    |
| 	PF7   | Left A distans sensor  |  `IRaL`  |   36    |
-------------------------------------------------------------


Arduino Leonardo pinout:

| **Arduino**    | **Function**     | **Code** | **Pin** |
|:-------------: | :---------------:|:--------:| :------:|
| digital pin 0  | floor sensor  	  |  `FbL`   |	20     |
| digital pin 1  | floor sensor     |  `FbR`   |    21   |
| digital pin 2  | floor sensor  	  |  `FaL`   |	19	   |
| digital pin 3  | floor sensor  	  |  `FaR`   |	18	   |
| digital pin 4  | distans sensor	  |  `IRb`   |    25   |
| digital pin 5  | motor control	  |  `Mb2`   |	31     |
| digital pin 6  | motor PWM   		  |  `MaPWM` |    27   |
| digital pin 7  | built in LED  	  |`builtLed1`|    1   |
| digital pin 8  | motor control	  |  `Ma2`   |    28   |
| digital pin 9  | motor control	  |  `Ma1`   |    29   |
| digital pin 10 | motor control	  |  `Mb1`   |    30   |
| digital pin 11 | unplugged	  	  | 	---	   |    12   |
| digital pin 12 | distans sensor	  |  `IRbL`  |    26   |
|    analog 0    | distans sensor   |  `IRaL`  |    32   |
|    analog 1    | distans sensor	  |  `IRa`   |    33   |
|    analog 2    | distans sensor	  |  `IRaR`  |    34   |
|    analog 3    | button  		 	    |	 `but1`  |    35   |
|    analog 4    | button         	|  `but2`  |    36   |
|    analog 5    | button 			    |  `but3`  |    37   |
| 	 txLED 	     | distans sensor  	|  `IRbR`  |    22   |
| 	   HWB 	     | built in LED     |`builtLed2`|   33   |  
----------------------------------------------------------

Code definitions:

| 	**Group** 	 | **Code** |          **Definition**     	    |
|:--------------:|:--------:|				-					|
| Floor Sensors	 |   FbL	|				-					|
|		.		 |   FbR	|				-					|
|		.		 |   FaL	|				-					|
| 		.		 |   FaR	|				-					|
| 		.		 | 	 .      |				-					|
|Distans Senstors| IRaL	    |				-					|
| 		.		 |  IRa     |				-					|
| 		.		 |  IRaR    |				-					|
| 		.		 |  IRbL	|				-					|
| 		.		 |  IRb     |				-					|
| 		.		 |  IRBR    |				-					|
| 		.		 | 	.       |				-					|
|Motors Control	 | 	Ma1     |				-					|
|		.		 | 	Ma2     |				-					|
|		.		 |	MaPWM   | 				-					|
|		.		 |	Mb1     |				-					|
|		.		 |	Mb2	    | 				-					|
|		.		 |	MbPWM   | 				-					|
|		.		 |	.	    |				-					|
|	Output 		 |builtLed1 |				-					|
|		.		 |builtLed2 |				-					|
-----------------------------------------------------------------



program0 empty
program1 empty
program2 spinner
program3 basic
program4 waiter
program5
program6 basic without floorSensors
program7 wheels cleaner
