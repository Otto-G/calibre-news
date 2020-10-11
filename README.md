# calibre-news

This repository contains some recipies to pull in news articles with the intent to send them to a Kindle device.  

## Missing files

There are some missing configuration files that need to be added in order to define how and to whom the articles are sent to.

sendmail.config: 
```bash
SMTP=smtp.gmail.com
PORT=587
USER=username@gmail.com
PASSWD=password
FROM=username@gmail.com
```

emails.txt:
```txt
email@kindle.com
```

## Command to run
 `docker exec -it -w /recipies calibre-web /recipies/propublica_fetch.sh`
