# Introduction

This application offers functions that may run automatically every time a goods receipt is created.

# Installation

You install the application from the connection view in Thetis IMS. The name of the application is 'thetis-ims-goods-receipt-utilities'.

# Configuration

In the data document of the context:

```
{
  "GoodsReceiptUtilities": {
    "createResidualInboundShipment": true,
    "residualInboundShipmentSuffix": "-R"
  }
}
```
# Options

#### createResidualInboundShipment

If this field is true, the application will automatically create a new inbound shipment containing that which was expected but not received.

#### residualInboundShipmentSuffix

The number of the new inbound shipment will be the the same as the old except from this suffix. 

