curl -v -X POST https://api.line.me/v2/bot/richmenu \
-H 'Authorization: Bearer L3eT/IDHbrBjaLuRM4IR+tgtCEatSQvlSk6Mawma4T7z0YGtEec6yf+K+X/OBoJifcW5OLGxKKi5wGM6W7HRV6vcZd+eP8K5JfNYzZ/jOGg+EzqiDl2o2b/CJDlUTyYmXBVhNLKRk0gZeWIynv3l9gdB04t89/1O/w1cDnyilFU=' \
-H 'Content-Type: application/json' \
-d \
'{
  "size": {
    "width": 2500,
    "height": 1686
   },
   "selected": true,
   "name": "Rich menu v1.0",
   "chatBarText": "Tap here",
   "areas": [
    {
      "bounds": {
        "x": 0,
        "y": 0,
        "width": 2500,
        "height": 1686
      },
      "action": {
        "type": "datetimepicker",
        "label":"Select date",
        "data":"storeId=12345",
        "mode":"date"
      }
    }
  ]
}'
