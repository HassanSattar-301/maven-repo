
# User

*This model accepts additional fields of type Object.*

## Structure

`User`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `Long` | Optional | - | Long getId() | setId(Long id) |
| `Username` | `String` | Optional | - | String getUsername() | setUsername(String username) |
| `FirstName` | `String` | Optional | - | String getFirstName() | setFirstName(String firstName) |
| `LastName` | `String` | Optional | - | String getLastName() | setLastName(String lastName) |
| `Email` | `String` | Optional | - | String getEmail() | setEmail(String email) |
| `Password` | `String` | Optional | - | String getPassword() | setPassword(String password) |
| `Phone` | `String` | Optional | - | String getPhone() | setPhone(String phone) |
| `UserStatus` | `Integer` | Optional | User Status | Integer getUserStatus() | setUserStatus(Integer userStatus) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example

```java
import io.swagger.petstore3.ApiHelper;
import io.swagger.petstore3.models.User;
import java.io.IOException;

User user = new User.Builder()
    .id(76L)
    .username("username0")
    .firstName("firstName4")
    .lastName("lastName4")
    .email("email6")
.additionalProperty("exampleAdditionalProperty", ApiHelper.deserialize("{\"key1\":\"val1\",\"key2\":\"val2\"}"))
    .build();
```

