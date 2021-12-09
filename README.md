# URL-shortener

URL Shortener made using Flask  

username: `admin`   
password: `password`   

Home Page:   
![](https://i.imgur.com/4BZ0lyl.jpg)

Input URL:  
![](https://i.imgur.com/6F3nbZr.png)

After Shortening:  
![](https://i.imgur.com/QOPoG4x.jpg)

Statistics:  
![](https://i.imgur.com/vjErV0M.jpg)

To run locally:  

```sh
git clone https://github.com/rith-vik-7/URL-shortener.git
cd URL-shortener/url_shortener
python3 -m pip flask
python3 -m pip install python-dotenv
python3 -m pip install flask-sqlalchemy
```

To set up database locally:  

```sh
python3
```

```py
from url shortener import create_ app
from url shortener.extensions import db
from url shortener.models import Link
db.create_all (app=create_app())
```

To check database:  
```sh
sqlite3 db.sqlite3
```

```sql
sqlite> .tables                                                                                                                                             
link                                                                                                                                                        
sqlite> select * from link;
1|https://github.com/rith-vik-7/URL-shortener/tree/main|K2L5nWt|4|2021-11-21 09:48:15.623871                                                                
2|https://timesofindia.indiatimes.com/world/china/china-plenum-what-to-know-about-xi-jinpings-doctrine-that-could-let-him-rule-for-life/articleshow/87578405
.cms|HWNxfiy|2|2021-11-21 10:00:01.234335                                                                                                                   
3|http://rithvik7.pythonanywhere.com|jUkbRkk|3|2021-11-21 10:17:28.344176                                                                                   
4|http://rithvik7.pythonanywhere.com|8os69XY|0|2021-11-21 10:17:47.732094                                                                                   
5|https://timesofindia.indiatimes.com/business/india-business/no-change-in-petrol-diesel-rates/articleshow/87827923.cms|JBjDWjs|1|2021-11-21 10:41:25.994713
6|https://google.com|JQ3chzh|1|2021-11-21 10:41:26.925336                                                                                                   
7|https://timesofindia.indiatimes.com/business/india-business/no-change-in-petrol-diesel-rates/articleshow/87827923.cms|eQNGwEP|0|2021-11-21 10:41:51.405011
8|https://google.com|Vm2gmQd|0|2021-11-21 10:55:02.083278                                                                                                   
9|https://github.com/rith-vik-7/URL-shortener/rith-vik-7/URL-shortener/tree/main|wAJ1R1T|1|2021-11-21 12:09:19.046480                                       
10|https://github.com/rith-vik-7/DIP-project|ikpSl38|2|2021-11-21 12:15:37.680920                                                                           
11|https://www.google.co.in/?client=safari|CSxScSI|0|2021-11-21 12:18:44.949687                                                                             
12|www.google.com|SEBG5lc|1|2021-11-21 12:19:19.310742                                                                                                      
13||ZSfe209|0|2021-11-21 12:21:11.319994                                                                                                                    
14|https://dominuto.herokuapp.com/|xpECwKV|0|2021-11-23 11:49:03.078657                                                                                     
15|https://google.com|US5cKoS|1|2021-11-30 09:39:51.999767                                                                                                  
16|https://hackmd.io/|4w1ViTb|0|2021-12-09 15:25:41.507876  
sqlite> DELETE from link where visits=0; 
sqlite> select * from link;                                                                                                                                 
1|https://github.com/rith-vik-7/URL-shortener/tree/main|K2L5nWt|4|2021-11-21 09:48:15.623871                                                                
2|https://timesofindia.indiatimes.com/world/china/china-plenum-what-to-know-about-xi-jinpings-doctrine-that-could-let-him-rule-for-life/articleshow/87578405
.cms|HWNxfiy|2|2021-11-21 10:00:01.234335                                                                                                                   
3|http://rithvik7.pythonanywhere.com|jUkbRkk|3|2021-11-21 10:17:28.344176                                                                                   
5|https://timesofindia.indiatimes.com/business/india-business/no-change-in-petrol-diesel-rates/articleshow/87827923.cms|JBjDWjs|1|2021-11-21 10:41:25.994713
6|https://google.com|JQ3chzh|1|2021-11-21 10:41:26.925336                                                                                                   
9|https://github.com/rith-vik-7/URL-shortener/rith-vik-7/URL-shortener/tree/main|wAJ1R1T|1|2021-11-21 12:09:19.046480                                       
10|https://github.com/rith-vik-7/DIP-project|ikpSl38|2|2021-11-21 12:15:37.680920                                                                           
12|www.google.com|SEBG5lc|1|2021-11-21 12:19:19.310742                                                                                                      
15|https://google.com|US5cKoS|1|2021-11-30 09:39:51.999767 
```                 

![](https://i.imgur.com/qDLFvxC.jpg)


