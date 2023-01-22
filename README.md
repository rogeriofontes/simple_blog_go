# simple_blog_go

go get .
go run .

--
curl http://localhost:8000/posts \
    --include \
    --header "Content-Type: application/json" \
    --request "GET"

curl --location --request GET 'http://localhost:8000/posts' \
--data-raw ''

curl http://localhost:8000/posts/P0111 \
    --include \
    --header "Content-Type: application/json" \
    --request "GET"

curl http://localhost:8000/posts \
    --include \
    --header "Content-Type: application/json" \
    --request "POST" \
    --data '{"title": "post2","body": "MacBook is gr"}'

curl --location --request POST 'http://localhost:8000/posts' \
--header 'Content-Type: application/json' \
--data-raw '{
    "body": "POSTSSSS2",
    "title": "post2"
}'
