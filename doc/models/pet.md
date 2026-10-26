
# Pet

*This model accepts additional fields of type Object.*

## Structure

`Pet`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `Long` | Optional | - | Long getId() | setId(Long id) |
| `Name` | `String` | Required | - | String getName() | setName(String name) |
| `Category` | [`Category`](../../doc/models/category.md) | Optional | - | Category getCategory() | setCategory(Category category) |
| `PhotoUrls` | `List<String>` | Required | - | List<String> getPhotoUrls() | setPhotoUrls(List<String> photoUrls) |
| `Tags` | [`List<Tag>`](../../doc/models/tag.md) | Optional | - | List<Tag> getTags() | setTags(List<Tag> tags) |
| `Status` | [`PetStatus`](../../doc/models/pet-status.md) | Optional | pet status in the store | PetStatus getStatus() | setStatus(PetStatus status) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example

```java
import io.swagger.petstore3.ApiHelper;
import io.swagger.petstore3.models.Category;
import io.swagger.petstore3.models.Pet;
import io.swagger.petstore3.models.PetStatus;
import io.swagger.petstore3.models.Tag;
import java.io.IOException;
import java.util.Arrays;

Pet pet = new Pet.Builder(
    "name0",
    Arrays.asList(
        "photoUrls5",
        "photoUrls6"
    )
)
.id(72L)
.category(new Category.Builder()
        .id(232L)
        .name("name2")
    .additionalProperty("exampleAdditionalProperty", ApiHelper.deserialize("{\"key1\":\"val1\",\"key2\":\"val2\"}"))
        .build())
.tags(Arrays.asList(
        new Tag.Builder()
            .id(26L)
            .name("name0")
        .additionalProperty("exampleAdditionalProperty", ApiHelper.deserialize("{\"key1\":\"val1\",\"key2\":\"val2\"}"))
            .build()
    ))
.status(PetStatus.AVAILABLE)
.additionalProperty("exampleAdditionalProperty", ApiHelper.deserialize("{\"key1\":\"val1\",\"key2\":\"val2\"}"))
.build();
```

