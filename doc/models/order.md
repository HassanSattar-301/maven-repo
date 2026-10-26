
# Order

*This model accepts additional fields of type Object.*

## Structure

`Order`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `Long` | Optional | - | Long getId() | setId(Long id) |
| `PetId` | `Long` | Optional | - | Long getPetId() | setPetId(Long petId) |
| `Quantity` | `Integer` | Optional | - | Integer getQuantity() | setQuantity(Integer quantity) |
| `ShipDate` | `LocalDateTime` | Optional | - | LocalDateTime getShipDate() | setShipDate(LocalDateTime shipDate) |
| `Status` | [`OrderStatus`](../../doc/models/order-status.md) | Optional | Order Status | OrderStatus getStatus() | setStatus(OrderStatus status) |
| `Complete` | `Boolean` | Optional | - | Boolean getComplete() | setComplete(Boolean complete) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example

```java
import io.swagger.petstore3.ApiHelper;
import io.swagger.petstore3.DateTimeHelper;
import io.swagger.petstore3.models.Order;
import io.swagger.petstore3.models.OrderStatus;
import java.io.IOException;

Order order = new Order.Builder()
    .id(144L)
    .petId(184L)
    .quantity(100)
    .shipDate(DateTimeHelper.fromRfc8601DateTime("2016-03-13T12:52:32.123Z"))
    .status(OrderStatus.PLACED)
.additionalProperty("exampleAdditionalProperty", ApiHelper.deserialize("{\"key1\":\"val1\",\"key2\":\"val2\"}"))
    .build();
```

