curl -v -X POST https://api.line.me/v2/bot/richmenu \
-H 'Authorization: Bearer L3eT/IDHbrBjaLuRM4IR+tgtCEatSQvlSk6Mawma4T7z0YGtEec6yf+K+X/OBoJifcW5OLGxKKi5wGM6W7HRV6vcZd+eP8K5JfNYzZ/jOGg+EzqiDl2o2b/CJDlUTyYmXBVhNLKRk0gZeWIynv3l9gdB04t89/1O/w1cDnyilFU=' \
-H 'Content-Type: application/json' \
-d \
'{
  "size": {
    "width": 2500,
    "height": 835
   },
   "selected": true,
   "name": "Rich menu v1.0",
   "chatBarText": "お問い合わせ",
   "areas": [
    {
      "bounds": {
        "x": 0,
        "y": 0,
        "width": 834,
        "height": 835
      },
      "action": {
        "type": "datetimepicker",
        "data":"storeId=12345",
        "mode":"date"
      }
    },
    {
      "bounds": {
        "x": 834,
        "y": 0,
        "width": 833,
        "height": 835
      },
      "action": {
        "type": "uri",
        "uri": "https://paperlink.jp/"
      }
    },
    {
      "bounds": {
        "x": 1667,
        "y": 0,
        "width": 833,
        "height": 835
      },
      "action": {
        "type": "uri",
        "uri": "https://paperlink.jp/"
      }
    },
  ]
}'

## response

Note: Unnecessary use of -X or --request, POST is already inferred.
*   Trying 203.104.153.64...
* TCP_NODELAY set
* Connected to api.line.me (203.104.153.64) port 443 (#0)
* ALPN, offering h2
* ALPN, offering http/1.1
* successfully set certificate verify locations:
*   CAfile: /etc/ssl/cert.pem
  CApath: none
* TLSv1.2 (OUT), TLS handshake, Client hello (1):
* TLSv1.2 (IN), TLS handshake, Server hello (2):
* TLSv1.2 (IN), TLS handshake, Certificate (11):
* TLSv1.2 (IN), TLS handshake, Server key exchange (12):
* TLSv1.2 (IN), TLS handshake, Server finished (14):
* TLSv1.2 (OUT), TLS handshake, Client key exchange (16):
* TLSv1.2 (OUT), TLS change cipher, Change cipher spec (1):
* TLSv1.2 (OUT), TLS handshake, Finished (20):
* TLSv1.2 (IN), TLS change cipher, Change cipher spec (1):
* TLSv1.2 (IN), TLS handshake, Finished (20):
* SSL connection using TLSv1.2 / ECDHE-RSA-AES256-GCM-SHA384
* ALPN, server accepted to use h2
* Server certificate:
*  subject: C=JP; ST=Tokyo-to; L=Shinjuku-ku; O=LINE Corporation; CN=*.line.me
*  start date: Jun 17 06:01:58 2020 GMT
*  expire date: Sep  5 12:00:00 2022 GMT
*  subjectAltName: host "api.line.me" matched cert's "*.line.me"
*  issuer: C=BE; O=GlobalSign nv-sa; CN=GlobalSign RSA OV SSL CA 2018
*  SSL certificate verify ok.
* Using HTTP2, server supports multi-use
* Connection state changed (HTTP/2 confirmed)
* Copying HTTP/2 data in stream buffer to connection buffer after upgrade: len=0
* Using Stream ID: 1 (easy handle 0x7ffc0080f800)
> POST /v2/bot/richmenu HTTP/2
> Host: api.line.me
> User-Agent: curl/7.64.1
> Accept: */*
> Authorization: Bearer L3eT/IDHbrBjaLuRM4IR+tgtCEatSQvlSk6Mawma4T7z0YGtEec6yf+K+X/OBoJifcW5OLGxKKi5wGM6W7HRV6vcZd+eP8K5JfNYzZ/jOGg+EzqiDl2o2b/CJDlUTyYmXBVhNLKRk0gZeWIynv3l9gdB04t89/1O/w1cDnyilFU=
> Content-Type: application/json
> Content-Length: 296
> 
* We are completely uploaded and fine
* Connection state changed (MAX_CONCURRENT_STREAMS == 128)!
< HTTP/2 200 
< server: openresty
< date: Sat, 06 Feb 2021 09:52:42 GMT
< content-type: application/json
< x-line-request-id: 6344557a-260d-46d8-bb8f-417169fecee0
< x-content-type-options: nosniff
< x-xss-protection: 1; mode=block
< cache-control: no-cache, no-store, max-age=0, must-revalidate
< pragma: no-cache
< expires: 0
< x-frame-options: DENY
< 
* Connection #0 to host api.line.me left intact
{"richMenuId":"richmenu-cb3ad2cd34d23376e4c54b5ed32c2be2"}* Closing connection 0
