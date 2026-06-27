# Local Waste Services (Central Ohio)

Support for schedules provided by [Local Waste Services](https://localwasteservices.com), including official residential service-guidelines pages and community directory entries.

## Configuration via configuration.yaml

```yaml
waste_collection_schedule:
  sources:
    - name: localwasteservices_com
      args:
        url: https://localwasteservices.com/service-guidelines/violet-township
```

### Configuration Variables

This source accepts either a direct `url` to a service-guidelines page or a `directory_url` plus `community_name` for resolving a page from the residential-services directory.

## Examples

Direct page:

```yaml
waste_collection_schedule:
  sources:
    - name: localwasteservices_com
      args:
        url: https://localwasteservices.com/service-guidelines/violet-township
```

Directory lookup:

```yaml
waste_collection_schedule:
  sources:
    - name: localwasteservices_com
      args:
        directory_url: https://localwasteservices.com/services/residential-services
        community_name: Violet Township
```
