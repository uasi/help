# cURL

## POST

curl -X POST -d data=$URL_ENCODED_DATA $URL
curl -X POST --data-urlencode data=$RAW_DATA $URL

## POST JSON

curl -X POST -H "Content-Type: application/json" -d $JSON_DATA $URL
