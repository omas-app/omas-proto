## omas proto

https://github.com/omas-app/omas-proto


## add protobuf reference
$proto="google\type\date.proto"
$url="https://raw.githubusercontent.com/googleapis/googleapis/master/$proto"
dotnet-grpc add-url $url --project src/Omas.Client --output $proto

## refresh protos
dotnet-grpc refresh --project src/Omas.Client


## bolt prmpt used
omas api aligns with google AIP spec the name field of vendor type and fullfilment type is an resource name and not the display name. the label field should be used for restaurant names. Omas api vendor type has an optional field vendor.info.atts['Cuisines'] with a string array with the restaurant Cuisines. vendor.tag field contains a string array with tags. the tag "delivery" means that the vendor accepts "delivery" and the tag "pickup" is for pockup order type. if none of them is specified then the vendor default can both delivery and pickup. The tag min-delivery-required is that the vendor only accept a min order amount even if a service-fee could be added. the vendor location can be used from the field vendor.loc[0]. If the tag delivery-cash is set then the vendor only accepts cash on delivery and not ATM card, if the delivery-card tag is set then the vendor accepts ATM card on delivery, if none of them is set then vendor accepts both delivery-cash and delivery-card. the vendor.deliveryZones field contains a array of DeliveryZone types with minPrice for the min order amount, serviceFee for the fixed delivery fee and serviceFeeMax for the amount when the delivery is free. the vendor.logo can be used inclduing the aspect ratio for the vendor logo and vendor.images contains a list of images where the image with the tag "ambient" can be used as the background ambient image. the Location type contains a field openHours it has Mo-So and a flag for holiday.

