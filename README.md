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
