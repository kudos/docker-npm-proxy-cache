## Usage

Run the container

```
docker run --net=host -p 8080:8080 -t kudoz/npm-proxy-cache
```

Use it with `npm`, replacing the npm-proxy-cache hostname below with the ip or hostname you have the container above running at.

```
npm --proxy http://npm-proxy-cache:8080 --https-proxy http://npm-proxy-cache:8080 --strict-ssl false install
```
