# HTTP request analysis notes

Use this file to record what you actually observe in Burp.

## Example request anatomy

For a request such as:

```http
GET /filter?category=Pets HTTP/2
Host: example-lab.invalid
Accept: text/html
```

- **Method:** `GET` requests a resource.
- **Path:** `/filter` identifies the route.
- **Query parameter:** `category=Pets` supplies an input value.
- **Host:** identifies the requested host.
- **Response status:** record the actual status from Burp, such as `200 OK`.
- **Response body:** summarize what the server returned without copying sensitive data.

The host above is illustrative, not a real lab address.

## My observation

- Date:
- Lab / authorized target:
- Burp tool:
- Request method and path:
- Parameter names (not sensitive values):
- Response status:
- Meaningful response difference:
- What I learned:
- Screenshot added (yes/no):
