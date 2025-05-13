# omas protobuf

## Description

A place to hold and share omas protobuf documents.

### Contribute

read the AIP Purpose and Guidelines
https://google.aip.dev


## dotnet

### Information

https://learn.microsoft.com/en-us/aspnet/core/grpc/dotnet-grpc?view=aspnetcore-8.0

### add protobuf reference

```pwsh
$proto="omas/v1/order.proto"
$url="https://raw.githubusercontent.com/omas-app/omas-proto/master/$proto"
dotnet-grpc add-url $url --project src/Omas.Client --output $proto
```

## ProtoJSON

### short forms

- name:resource_name
- n:display_name
- cn:common_name
- s?slug,sender
- r:receiver
- fid:foreign_id
- k:key
- sub:subject
- nr:number
- o:option
- i:info
- v:value
- vn:vendor
- tn:tenant
- u:user
- desc:description
- attr:attribute
- atts:attributes
- ts:timestamp
- msg:message
- meta:metadata
- c:contact
- a:amount
- ccy:currency
- q:quantity
- t:total
- rev:revision
- seq:sequence
- hdr:header
- hdrs:headers
- vals:values
- opts:options
- cts:created_at
- mts:modified_at
- loc:location
- addr:address
- thumbs:thumbnails
- del:deleted
- sort:sort_order
- p:price
- sel:selectors
- f:filter
- excl:exclusions