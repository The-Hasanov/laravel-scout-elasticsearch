### Lumen
While working in production, to keep your existing search experience available while reimporting your data, you also can use `scout:import` Artisan command:  

```
$app->register(\Matchish\ScoutElasticSearch\ElasticSearchServiceProvider::class);
$app->register(\Matchish\ScoutElasticSearch\ScoutElasticSearchServiceProvider::class);
```

The command create new temporary index, import all models to it, and then switch to the index and remove old index.
