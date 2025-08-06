
V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/workspace (develop/vvs)
$ grpcurl -plaintext \
  -H "online-feature-store-caller-id: test" \
  -H "online-feature-store-auth-token: test" \
  -d @ \
  localhost:8089 persist.FeatureService/PersistFeatures < persist.json
bash: persist.json: No such file or directory

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/workspace (develop/vvs)
$ cd .

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/workspace (develop/vvs)
$ cd ..

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start (develop/vvs)
$ grpcurl -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -d @   localhost:8089 persist.FeatureService/PersistFeatures < persist-sample.json
bash: persist-sample.json: No such file or directory

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start (develop/vvs)
$ cd sample-data

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -d @   localhost:8089 persist.FeatureService/PersistFeatures < persist-sample.json
Error invoking method "persist.FeatureService/PersistFeatures": error getting request data: message type persist.Query has no known field named feature_groups

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ ^[[200~grpcurl -v -plaintext \
>   -H "online-feature-store-caller-id: test" \
>   -H "online-feature-store-auth-token: test" \
>   -format json \
>   -d @ \
>   localhost:8089 persist.FeatureService/PersistFeatures < persist-sample.json
bash: $'\E[200~grpcurl': command not found

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ ~grpcurl -v -plaintext \
  -H "online-feature-store-caller-id: test" \
  -H "online-feature-store-auth-token: test" \
  -format json \
  -d @ \
  localhost:8089 persist.FeatureService/PersistFeatures < persist-sample.json
bash: ~grpcurl: command not found

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 persist.FeatureService/PersistFeatures < persist-sample.json

Resolved method descriptor:
rpc PersistFeatures ( .persist.Query ) returns ( .persist.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test
Error invoking method "persist.FeatureService/PersistFeatures": error getting request data: message type persist.Query has no known field named feature_groups

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 persist.FeatureService/PersistFeatures < persist-sample.json

Resolved method descriptor:
rpc PersistFeatures ( .persist.Query ) returns ( .persist.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test

Response headers received:
(empty)

Response trailers received:
content-type: application/grpc
Sent 1 request and received 0 responses
ERROR:
  Code: Unknown
  Message: failed to get feature group user_features: feature group user_features not found

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ ^C

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 persist.FeatureService/PersistFeatures < persist-sample.json

Resolved method descriptor:
rpc PersistFeatures ( .persist.Query ) returns ( .persist.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test

Response headers received:
(empty)

Response trailers received:
content-type: application/grpc
Sent 1 request and received 0 responses
ERROR:
  Code: Unknown
  Message: failed to parse feature value for entity catalog and feature group int_id_mapping: fp32_values is nil

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 persist.FeatureService/PersistFeatures < persist-sample.json

Resolved method descriptor:
rpc PersistFeatures ( .persist.Query ) returns ( .persist.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test
Error invoking method "persist.FeatureService/PersistFeatures": error getting request data: message type persist.Values has no known field named f32_values

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 persist.FeatureService/PersistFeatures < persist-sample.json

Resolved method descriptor:
rpc PersistFeatures ( .persist.Query ) returns ( .persist.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test

Response headers received:
content-type: application/grpc

Response contents:
{
  "message": "Data Persisted Successfully"
}

Response trailers received:
(empty)
Sent 1 request and received 1 response

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ ^C

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext \
  -H "online-feature-store-caller-id: test" \
  -H "online-feature-store-auth-token: test" \
  -format json \
  -d @ \
  localhost:8089 fetch.FeatureService/FetchFeatureValues < retrieve-request.json
bash: retrieve-request.json: No such file or directory

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 fetch.FeatureService/FetchFeatureValues < retrieve-sample.json
Error invoking method "fetch.FeatureService/FetchFeatureValues": target server does not expose service "fetch.FeatureService"

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 fetch.FeatureService/FetchFeatureValues < retrieve-sample.json
Error invoking method "fetch.FeatureService/FetchFeatureValues": target server does not expose service "fetch.FeatureService"

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 fetch.FeatureService/FetchFeatureValues < retrieve-sample.json
Error invoking method "fetch.FeatureService/FetchFeatureValues": target server does not expose service "fetch.FeatureService"

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 fetch.FeatureService/FetchFeatureValues < retrieve-sample.json
Error invoking method "fetch.FeatureService/FetchFeatureValues": target server does not expose service "fetch.FeatureService"

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 fetch.FeatureService/FetchFeatureValues < retrieve-sample.json
Error invoking method "fetch.FeatureService/FetchFeatureValues": target server does not expose service "fetch.FeatureService"

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 persist.FeatureService/PersistFeatures < persist-sample.json

Resolved method descriptor:
rpc PersistFeatures ( .persist.Query ) returns ( .persist.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test

Response headers received:
content-type: application/grpc

Response contents:
{
  "message": "Data Persisted Successfully"
}

Response trailers received:
(empty)
Sent 1 request and received 1 response

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 fetch.FeatureService/FetchFeatureValues < retrieve-sample.json
Error invoking method "fetch.FeatureService/FetchFeatureValues": target server does not expose service "fetch.FeatureService"

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext \
  -H "online-feature-store-caller-id: test" \
  -H "online-feature-store-auth-token: test" \
  -format json \
  -d @ \
  localhost:8089 fetch.FeatureService/FetchFeatureValues < retrieve-sample.json
Error invoking method "fetch.FeatureService/FetchFeatureValues": target server does not expose service "fetch.FeatureService"

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ ^C

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -plaintext localhost:8089 list
grpc.reflection.v1.ServerReflection
grpc.reflection.v1alpha.ServerReflection
p2p.P2PCacheService
persist.FeatureService
retrieve.FeatureService

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ ^C

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext \
  -H "online-feature-store-caller-id: test" \
  -H "online-feature-store-auth-token: test" \
  -format json \
  -d @ \
  localhost:8089 retrieve.FeatureService/FetchFeatureValues < retrieve-sample.json
Error invoking method "retrieve.FeatureService/FetchFeatureValues": service "retrieve.FeatureService" does not include a method named "FetchFeatureValues"

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 persist.FeatureService/PersistFeatures < persist-sample.json

Resolved method descriptor:
rpc PersistFeatures ( .persist.Query ) returns ( .persist.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test

Response headers received:
content-type: application/grpc

Response contents:
{
  "message": "Data Persisted Successfully"
}

Response trailers received:
(empty)
Sent 1 request and received 1 response

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 retrieve.FeatureService/FetchFeatureValues < retrieve-sample.json
Error invoking method "retrieve.FeatureService/FetchFeatureValues": service "retrieve.FeatureService" does not include a method named "FetchFeatureValues"

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ ^C

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -plaintext localhost:8089 list retrieve.FeatureService
retrieve.FeatureService.RetrieveDecodedResult
retrieve.FeatureService.RetrieveFeatures

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ ^C

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -plaintext localhost:8089 describe retrieve.FeatureService.RetrieveFeatures
retrieve.FeatureService.RetrieveFeatures is a method:
rpc RetrieveFeatures ( .retrieve.Query ) returns ( .retrieve.Result );

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ ^C

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext \
  -H "online-feature-store-caller-id: test" \
  -H "online-feature-store-auth-token: test" \
  -format json \
  -d @ \
  localhost:8089 retrieve.FeatureService/RetrieveFeatures < retrieve-sample.json

Resolved method descriptor:
rpc RetrieveFeatures ( .retrieve.Query ) returns ( .retrieve.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test
Error invoking method "retrieve.FeatureService/RetrieveFeatures": error getting request data: message type retrieve.Query has no known field named key_values

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ ^C

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -plaintext localhost:8089 describe retrieve.Query
retrieve.Query is a message:
message Query {
  string entity_label = 1;
  repeated .retrieve.FeatureGroup feature_groups = 2;
  repeated string keys_schema = 3;
  repeated .retrieve.Keys keys = 4;
}

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ ^C

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 retrieve.FeatureService/RetrieveFeatures < retrieve-sample.json

Resolved method descriptor:
rpc RetrieveFeatures ( .retrieve.Query ) returns ( .retrieve.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test
Error invoking method "retrieve.FeatureService/RetrieveFeatures": error getting request data: message type retrieve.Keys has no known field named key_values

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 persist.FeatureService/PersistFeatures < persist-sample.json

Resolved method descriptor:
rpc PersistFeatures ( .persist.Query ) returns ( .persist.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test

Response headers received:
content-type: application/grpc

Response contents:
{
  "message": "Data Persisted Successfully"
}

Response trailers received:
(empty)
Sent 1 request and received 1 response

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext \
  -H "online-feature-store-caller-id: test" \
  -H "online-feature-store-auth-token: test" \
  -format json \
  -d @ \
  localhost:8089 retrieve.FeatureService/RetrieveFeatures < retrieve-sample.json

Resolved method descriptor:
rpc RetrieveFeatures ( .retrieve.Query ) returns ( .retrieve.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test
Error invoking method "retrieve.FeatureService/RetrieveFeatures": error getting request data: message type retrieve.Keys has no known field named key_values

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ ^C

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -plaintext localhost:8089 describe retrieve.Keys
retrieve.Keys is a message:
message Keys {
  repeated string cols = 1;
}

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ ^C

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 retrieve.FeatureService/RetrieveFeatures < retrieve-sample.json

Resolved method descriptor:
rpc RetrieveFeatures ( .retrieve.Query ) returns ( .retrieve.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test

Response headers received:
content-type: application/grpc

Response contents:
{
  "entityLabel": "catalog",
  "keysSchema": [
    "catalog_id"
  ],
  "featureSchemas": [
    {
      "featureGroupLabel": "int_id_mapping",
      "features": [
        {
          "label": "cat_id"
        }
      ]
    }
  ],
  "rows": [
    {
      "keys": [
        "some_catalog_id"
      ],
      "columns": [
        "AORARg=="
      ]
    }
  ]
}

Response trailers received:
(empty)
Sent 1 request and received 1 response

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 persist.FeatureService/PersistFeatures < persist-sample.json

Resolved method descriptor:
rpc PersistFeatures ( .persist.Query ) returns ( .persist.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test

Response headers received:
content-type: application/grpc

Response contents:
{
  "message": "Data Persisted Successfully"
}

Response trailers received:
(empty)
Sent 1 request and received 1 response

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 retrieve.FeatureService/RetrieveFeatures < retrieve-sample.json

Resolved method descriptor:
rpc RetrieveFeatures ( .retrieve.Query ) returns ( .retrieve.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test

Response headers received:
content-type: application/grpc

Response contents:
{
  "entityLabel": "catalog",
  "keysSchema": [
    "catalog_id"
  ],
  "featureSchemas": [
    {
      "featureGroupLabel": "int_id_mapping",
      "features": [
        {
          "label": "cat_id"
        }
      ]
    }
  ],
  "rows": [
    {
      "keys": [
        "some_catalog_id"
      ],
      "columns": [
        "AORARg=="
      ]
    }
  ]
}

Response trailers received:
(empty)
Sent 1 request and received 1 response

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ ^C

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 retrieve.FeatureService/RetrieveFeatures < retrieve-sample.json

Resolved method descriptor:
rpc RetrieveFeatures ( .retrieve.Query ) returns ( .retrieve.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test

Response headers received:
content-type: application/grpc

Response contents:
{
  "entityLabel": "catalog",
  "keysSchema": [
    "catalog_id"
  ],
  "featureSchemas": [
    {
      "featureGroupLabel": "int_id_mapping",
      "features": [
        {
          "label": "cat_id"
        }
      ]
    }
  ],
  "rows": [
    {
      "keys": [
        "10"
      ],
      "columns": [
        "AAAAAA=="
      ]
    }
  ]
}

Response trailers received:
(empty)
Sent 1 request and received 1 response

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 retrieve.FeatureService/RetrieveFeatures < retrieve-sample.json

Resolved method descriptor:
rpc RetrieveFeatures ( .retrieve.Query ) returns ( .retrieve.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test

Response headers received:
content-type: application/grpc

Response contents:
{
  "entityLabel": "catalog",
  "keysSchema": [
    "catalog_id"
  ],
  "featureSchemas": [
    {
      "featureGroupLabel": "int_id_mapping",
      "features": [
        {
          "label": "cat_id"
        }
      ]
    }
  ],
  "rows": [
    {
      "keys": [
        "some_catalog_id"
      ],
      "columns": [
        "AORARg=="
      ]
    }
  ]
}

Response trailers received:
(empty)
Sent 1 request and received 1 response

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 persist.FeatureService/PersistFeatures < persist-sample.json

Resolved method descriptor:
rpc PersistFeatures ( .persist.Query ) returns ( .persist.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test

Response headers received:
content-type: application/grpc

Response contents:
{
  "message": "Data Persisted Successfully"
}

Response trailers received:
(empty)
Sent 1 request and received 1 response

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 retrieve.FeatureService/RetrieveFeatures < retrieve-sample.json\
> grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 retrieve.FeatureService/RetrieveFeatures < retrieve-sample.json\
> exit
bash: retrieve-sample.jsongrpcurl: No such file or directory

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 retrieve.FeatureService/RetrieveFeatures < retrieve-sample.json

Resolved method descriptor:
rpc RetrieveFeatures ( .retrieve.Query ) returns ( .retrieve.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test

Response headers received:
content-type: application/grpc

Response contents:
{
  "entityLabel": "catalog",
  "keysSchema": [
    "catalog_id"
  ],
  "featureSchemas": [
    {
      "featureGroupLabel": "int_id_mapping",
      "features": [
        {
          "label": "cat_id"
        }
      ]
    }
  ],
  "rows": [
    {
      "keys": [
        "some_catalog_id"
      ],
      "columns": [
        "AORARg=="
      ]
    }
  ]
}

Response trailers received:
(empty)
Sent 1 request and received 1 response

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 persist.FeatureService/PersistFeatures < persist-sample.json

Resolved method descriptor:
rpc PersistFeatures ( .persist.Query ) returns ( .persist.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test

Response headers received:
content-type: application/grpc

Response contents:
{
  "message": "Data Persisted Successfully"
}

Response trailers received:
(empty)
Sent 1 request and received 1 response

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 retrieve.FeatureService/RetrieveFeatures < retrieve-sample.json

Resolved method descriptor:
rpc RetrieveFeatures ( .retrieve.Query ) returns ( .retrieve.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test

Response headers received:
content-type: application/grpc

Response contents:
{
  "entityLabel": "catalog",
  "keysSchema": [
    "catalog_id"
  ],
  "featureSchemas": [
    {
      "featureGroupLabel": "int_id_mapping",
      "features": [
        {
          "label": "cat_id"
        }
      ]
    }
  ],
  "rows": [
    {
      "keys": [
        "some_catalog_id"
      ],
      "columns": [
        "AORARg=="
      ]
    }
  ]
}

Response trailers received:
(empty)
Sent 1 request and received 1 response

V.Ashok@LAPTOP-D0BA5CIS MINGW64 /d/Meesho/BharatMlStack/quick-start/sample-data (develop/vvs)
$ grpcurl -v -plaintext   -H "online-feature-store-caller-id: test"   -H "online-feature-store-auth-token: test"   -format json   -d @   localhost:8089 persist.FeatureService/PersistFeatures < persist-sample.json

Resolved method descriptor:
rpc PersistFeatures ( .persist.Query ) returns ( .persist.Result );

Request metadata to send:
online-feature-store-auth-token: test
online-feature-store-caller-id: test

Response headers received:
content-type: application/grpc

Response contents:
{
  "message": "Data Persisted Successfully"
}

Response trailers received:
(empty)
Sent 1 request and received 1 response
