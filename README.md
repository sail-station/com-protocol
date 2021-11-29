# SAIL STATION OPEN COMUNICATION PROTOCOL #

This repo aims to provide an **Open Standard for UHF / VHF & HF to sailing vessels** during ocean crossing

### COM-PROTOCOL  *Basic Standard*

1. Read/Copy the vessel that looks for information (CODE-SIGN, LAT, LONG, COURSE, STREAK) 
   
   EX: PR2585, 25.27S, 38.04W, 165C, 125M

2. Ask if the vessel received weather information in the last 24hrs (if the answer is positive jump to rule 5, otherwise go to RULE3)

3. INFORM WEATHER in the following standard. This can be fetched from [WEATHER-PROTOCOL](https://github.com/sail-station/weather-protocol)

  - One line of weather report every 30s
  - Ask if the Vessel received the latest weather-line report
  - In case of negative answer repeat the line
  - Inform the next 48hrs of Weather Report in the following standard repeating 1-Line every 30s

|HR|WIND|GUST|DIRECTION|WAVE|DIRECTION|CLOUD|CLOUD TYPE|CAPE|COURSE SUGGEST|
|----|----|----|----|----|----|----|----|----|----|
|00|23|G34|NNE|2,4M|NNE|30|CB|000|120|
|06|24|G37|N|2,6M|N|30|CB|300|175|
|12|26|G40|N|2,6M|N|25|CB|550|175|
|18|24|G38|N|2,8M|N|20|CB|400|175|

  ![CLOUD TYPES](https://upload.wikimedia.org/wikipedia/commons/5/57/Cloud_types_en.svg)
  
 4. READ/COPY Vessel/Crew Status Report
 5. 
