DataStore has a few optional configurations, such as the ability to specify a custom conflict handler that runs if a mutation is rejected by AWS AppSync during one of the conflict resolution strategies.

You can also configure the number of records to sync as an upper bound on items (per-Model) which will be stored locally on the device, as well as a custom interval in minutes which is an override of the default 24 hour "base query" which runs as part of the Delta Sync process.

### Example

The code below illustrates a conflict resolution handler for the `Post` model that retries a mutation with the same title, but the most recent remote data for all other fields. The conflict resolution handler discards conflicts for all other models.

```dart
TBD
```