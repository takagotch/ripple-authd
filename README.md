### ripple-authd
---
https://github.com/ripple/ripple-authd

```js
message AuthData {
  
  message Server {
    required string host = 1;
    
    required uint256 correction = 2;
    
    optional uint256 verify = 3;
  }
  
  repeated Server server = 1;
}


message HostInfo {
  
  required uint256 hostid = 1;
}

message Challenge {
  
  required uint32 timestamp = 1;
  
  required uint256 unique = 2;
  
  required uint32 nonce = 3;
  
  message Server {
  
    required uint256 hostid = 1;
  }
  
  repeated Server server = 4;
}
```

```sh
git clone [repo url] ripple-authd
cd ripple-authd
npm install
cp config-example.js config.js
npm run gen
node app
```

```
```


