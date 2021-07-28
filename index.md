## BelElect

### A corpus for bias detetion in Russian and Belorussian languages

### Data
BelElect corpus has been created from Telegram posts on Belorussian chanels:
 - TUT.BY
 - belamova
 - Belarus Seychas
 - BelSat
 - ONT_NEWS
 - BetTA
 - Pool_1
 - Zheltye SLIVY

The data have been downloaded using the built-in function of the Telegram messenger. Date of download: 15.04.2021. Data from all channels contain posts from 1.08.2020 to 14.04.2021.
The image and video download limited to 8 MB.

### Format
The built-in chat download function of the Telegram messenger offers two option for download: HTML or JSON format. We chose JSON for this corpus.

The JSON-files start with channel metadata:   
"name": "channel_name",  
 "type": "public_channel",  
 "id": channel-id-number,  
 "messages": []  

Every message in the message list is structured as follows:   
"id": message_id_number,  
"type": "message",  
"date": message_date,  
"edited": date_edited,  
"from": chanel_name,  
"from_id": chanel_id,  
"text": message_text  
   
Some messages also contain photos and/or videos:

...   
"photo": "picture.jpg",   
"width": 496,   
"height": 625,   
... 

...   
"file": "(File not included. Change data exporting settings to download.)",   
"thumbnail": "(File not included. Change data exporting settings to download.)",
"media_type": "video_file",   
"mime_type": "video/mp4",   
"duration_seconds": seconds_number,   
"width": 640,   
"height": 480,   
...   

You can download the data [here](https://github.com/sviatlanahoehn/BelElect/blob/main/README.md)

### Reference
In you use this resource, please cite our paper:

S. Höhn, N. Asher, S. Mauw. (2021) Examining Linguistic Biases in Telegram with a Game Theoretic Analysis. In proceedings of the 3rd Multidisciplinary International Symposium on Disinformation in Open Online Media (MISDOOM).

@inproceedidngs{hoehnetal:2021:misdoom,  
author  = {H\"{o}hn, Sviatlana and Asher, Nicholas and Mauw, Sjouke},  
 year  = {2021},   
 title  = { Examining Linguistic Biases in Telegram with a Game Theoretic Analysis},   
 booktitle  = {Proceedings of the 3rd Multidisciplinary International Symposium on Disinformation in Open Online Media (MISDOOM)}   
}

