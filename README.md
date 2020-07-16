# Curl Crash Course - By Traversy Media

```c
// Simple GET Request
curl https://jsonplaceholder.typicode.com/posts
curl https://jsonplaceholder.typicode.com/posts/1

// Include HTTP Header (--include, -i)
curl --include https://jsonplaceholder.typicode.com/posts/1

// Header Only (--head, -I)
curl --head https://jsonplaceholder.typicode.com/posts/1

// Write output to file (-o, --output)
curl -o test.txt https://jsonplaceholder.typicode.com/posts/1

// Download File (-O, --remote-name)
curl -O http://i.imgur.com/QRlAg0b.png

// Limit Transfer Rate
curl -O --limit-rate 1000B http://i.imgur.com/QRlAg0b.png

// Spoof user agent
curl -O test.txt http://traversymedia.com/test.txt -A "Mozilla"

//  POST Data (-d, --data)
curl -d "title=Hello&body=Hello World" https://jsonplaceholder.typicode.com/posts

//  PUT Data (-X PUT -d)
curl -X PUT -d "title=Hello&body=Hello World" https://jsonplaceholder.typicode.com/posts/1

//  Delete Data (-X DELETE)
curl -X DELETE https://jsonplaceholder.typicode.com/posts/1

// Secured Routes
curl -u brad:mypassword https://jsonplaceholder.typicode.com/posts/1

// Follow Redirection (-L)
curl http://google.com
curl -L http://google.com

// Download Files From FTP Server
$ curl -u ftpuser:ftppass -O ftp://x.x.x.x/public_html/sopmefile.php

// Upload via FTP
curl -u test@traversymedia.com:123456! -T hello.txt ftp://ftp.traversymedia.com

// Download via FTP
curl -u test@traversymedia.com:123456! -O ftp://ftp.traversymedia.com/hello.txt
```

