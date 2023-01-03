# Hướng dẫn 
    Cấu hình trong file ocelot.json
    Cấu hình đích
```json
    "DownstreamPathTemplate": "/{everything}",
    "DownstreamScheme": "http",
    "DownstreamHostAndPorts": [
        {
        "Host": "172.20.7.18",
        "Port": 5432
        }
    ],
```

    Cấu hình nguồn
```json
    "UpstreamHttpMethod": [
        "Get",
        "Post"
    ],
    "UpstreamPathTemplate": "/request/{everything}"
```

# Config project
//Todo: Ocelot