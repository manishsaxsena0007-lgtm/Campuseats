# HTTP Request/Response Log

## Request 1 — Get Post 1

### Command

```bash
curl.exe -i https://jsonplaceholder.typicode.com/posts/1

HTTP/1.1 200 OK
Date: Sun, 16 Aug 2026 09:02:57 GMT
Content-Type: application/json; charset=utf-8
Content-Length: 292
Connection: keep-alive
access-control-allow-credentials: true
Cache-Control: max-age=43200
etag: W/"124-yiKdLzqO5gfBrJFrcdJ8Yq0LGnU"
expires: -1
pragma: no-cache
Server: cloudflare
vary: Origin, Accept-Encoding
via: 2.0 heroku-router
x-content-type-options: nosniff
x-powered-by: Express
x-ratelimit-limit: 1000
x-ratelimit-remaining: 999
Age: 15354
Accept-Ranges: bytes
cf-cache-status: HIT
CF-RAY: a2bf43581d2cffa9-BOM
alt-svc: h3=":443"; ma=86400

{
  "userId": 1,
  "id": 1,
  "title": "sunt aut facere repellat provident occaecati excepturi optio reprehenderit",
  "body": "quia et suscipit\nsuscipit recusandae consequuntur expedita et cum\nreprehenderit molestiae ut ut quas totam\nnostrum rerum est autem sunt rem eveniet architecto"
}

## Request 2 - Get user 1

### Command

```bash
curl.exe -i https://jsonplaceholder.typicode.com/users/1

HTTP/1.1 200 OK
Date: Sun, 16 Aug 2026 09:28:07 GMT
Content-Type: application/json; charset=utf-8
Content-Length: 509
Connection: keep-alive
access-control-allow-credentials: true
Cache-Control: max-age=43200
etag: W/"1fd-+2Y3G3w049iSZtw5t1mzSnunngE"
expires: -1
pragma: no-cache
Server: cloudflare
vary: Origin, Accept-Encoding
via: 2.0 heroku-router
x-content-type-options: nosniff
x-powered-by: Express
x-ratelimit-limit: 1000
x-ratelimit-remaining: 999
x-ratelimit-reset: 1786354974
Age: 26152
Accept-Ranges: bytes
cf-cache-status: HIT
CF-RAY: a2bf683979ad4419-BOM
alt-svc: h3=":443"; ma=86400

{
  "id": 1,
  "name": "Leanne Graham",
  "username": "Bret",
  "email": "Sincere@april.biz",
  "address": {
    "street": "Kulas Light",
    "suite": "Apt. 556",
    "city": "Gwenborough",
    "zipcode": "92998-3874",
    "geo": {
      "lat": "-37.3159",
      "lng": "81.1496"
    }
  },
  "phone": "1-770-736-8031 x56442",
  "website": "hildegard.org",
  "company": {
    "name": "Romaguera-Crona",
    "catchPhrase": "Multi-layered client-server neural-net",
    "bs": "harness real-time e-markets"
  }
}

---

## Request 3 — Get Comment 1

### Command

```bash
curl.exe -i https://jsonplaceholder.typicode.com/comments/1
```

### Response

```text
HTTP/1.1 200 OK
Date: Sun, 16 Aug 2026 09:42:17 GMT
Content-Type: application/json; charset=utf-8
Content-Length: 268
Connection: keep-alive
access-control-allow-credentials: true
Cache-Control: max-age=43200
etag: W/"10c-KJ4I9RM/+33TKdV8CFsIvqsDSP0"
expires: -1
pragma: no-cache
Server: cloudflare
vary: Origin, Accept-Encoding
via: 2.0 heroku-router
x-content-type-options: nosniff
x-powered-by: Express
x-ratelimit-limit: 1000
x-ratelimit-remaining: 999
x-ratelimit-reset: 1786867722
Age: 5672
Accept-Ranges: bytes
cf-cache-status: HIT
CF-RAY: a2bf7cf52adf37a5-BOM
alt-svc: h3=":443"; ma=86400

{
  "postId": 1,
  "id": 1,
  "name": "id labore ex et quam laborum",
  "email": "Eliseo@gardner.biz",
  "body": "laudantium enim quasi est quidem magnam voluptate ipsam eos\ntempora quo necessitatibus\ndolor quam autem quasi\nreiciendis et nam sapiente accusantium"
}
```

### Annotation

- **Status:** `200 OK` — The request was successful and the requested comment was found.
- **Content-Type:** `application/json; charset=utf-8` — The response contains JSON data encoded using UTF-8.

---

## Request 4 — Get Album 1

### Command

```bash
curl.exe -i https://jsonplaceholder.typicode.com/albums/1
```

### Response

```text
HTTP/1.1 200 OK
Date: Sun, 16 Aug 2026 09:44:00 GMT
Content-Type: application/json; charset=utf-8
Content-Length: 64
Connection: keep-alive
access-control-allow-credentials: true
Cache-Control: max-age=43200
etag: W/"40-74G1+b66MteeTYAz6G+NybtDGFA"
expires: -1
pragma: no-cache
Server: cloudflare
vary: Origin, Accept-Encoding
via: 2.0 heroku-router
x-content-type-options: nosniff
x-powered-by: Express
x-ratelimit-limit: 1000
x-ratelimit-remaining: 999
x-ratelimit-reset: 1785412056
Age: 22364
Accept-Ranges: bytes
cf-cache-status: HIT
CF-RAY: a2bf7f7cc9702c7b-BOM
alt-svc: h3=":443"; ma=86400

{
  "userId": 1,
  "id": 1,
  "title": "quidem molestiae enim"
}
```

### Annotation

- **Status:** `200 OK` — The request was successful and the requested album was found.
- **Content-Type:** `application/json; charset=utf-8` — The response contains JSON data encoded using UTF-8.

---

## Request 5 — Non-existent Post

### Command

```bash
curl.exe -i https://jsonplaceholder.typicode.com/posts/999999
```

### Response

```text
HTTP/1.1 404 Not Found
Date: Sun, 16 Aug 2026 09:45:11 GMT
Content-Type: application/json; charset=utf-8
Content-Length: 2
Connection: keep-alive
access-control-allow-credentials: true
Cache-Control: max-age=43200
etag: W/"2-vyGp6PvFo4RvsFtPoIWeCReyIC8"
expires: -1
pragma: no-cache
Server: cloudflare
vary: Origin, Accept-Encoding
via: 2.0 heroku-router
x-content-type-options: nosniff
x-powered-by: Express
x-ratelimit-limit: 1000
x-ratelimit-remaining: 999
x-ratelimit-reset: 1786865382
Age: 8163
cf-cache-status: HIT
CF-RAY: a2bf81379bf73f91-BOM
alt-svc: h3=":443"; ma=86400

{}
```

### Annotation

- **Status:** `404 Not Found` — The server could not find the requested resource. This request deliberately asked for a post that does not exist.
- **Content-Type:** `application/json; charset=utf-8` — The response body is in JSON format and uses UTF-8 encoding.