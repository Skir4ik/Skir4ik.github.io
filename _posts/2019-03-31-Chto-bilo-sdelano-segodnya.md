---
layout: post
title:  Что было сделано сегодня
category: News 
description: Работы было много, но оно того стоило...
---
<p>
1)Научился работать с Jekyll <br>
2)Создал сайт <br>
3)Вспомнил немножко html <br>
</p>

```python
import csv
authorsEmail = {}
with open( "calculator.history", "rt" ) as file:
    reader = csv.reader( file )
    for row in reader:
        name = row[0]
        email = row[1]
        if name not in authorsEmail:
            authorsEmail[ name ] = []
        emailList = authorsEmail[ name ]
        if email not in emailList:
            emailList.append( email )
for name, email in authorsEmail.items():
    print name, email
```


