
# Api Response

*This model accepts additional fields of type Object.*

## Structure

`ApiResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Code` | `Integer` | Optional | - | Integer getCode() | setCode(Integer code) |
| `Type` | `String` | Optional | - | String getType() | setType(String type) |
| `Message` | `String` | Optional | - | String getMessage() | setMessage(String message) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example

```java
import io.swagger.petstore3.ApiHelper;
import io.swagger.petstore3.models.ApiResponse;
import java.io.IOException;

ApiResponse apiResponse = new ApiResponse.Builder()
    .code(146)
    .type("type4")
    .message("message4")
.additionalProperty("exampleAdditionalProperty", ApiHelper.deserialize("{\"key1\":\"val1\",\"key2\":\"val2\"}"))
    .build();
```

