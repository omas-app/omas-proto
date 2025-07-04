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
- label:display_name
- cn:common_name
- fid:foreign_id
- sub:subject
- nr:number
- opt:option
- val:value
- desc:description
- attr:attribute
- atts:attributes
- ts:timestamp
- msg:message
- meta:metadata
- ccy:currency
- qty:quantity
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
- pr:price
- sel:selectors
- flt:filter
- excl:exclusions

### legacy short forms

because of some tooling short comings, 
single char property names are not benificial.

- n:display_name => label
- s:slug,sender
- r:receiver
- k:key
- o:option => opt
- i:info
- v:value => val
- vn:vendor
- tn:tenant
- u:user
- c:contact
- a:amount
- q:quantity => qty
- t:total
- p:price => pr
- f:filter => flt