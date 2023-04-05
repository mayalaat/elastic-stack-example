## Run

```
docker compose up -d elasticsearch
```

## Sample data

https://www.elastic.co/guide/en/kibana/7.1/tutorial-load-dataset.html#_load_the_data_sets

```bash
curl -O https://download.elastic.co/demos/kibana/gettingstarted/7.x/logs.jsonl.gz
```

```bash
curl -H 'Content-Type: application/x-ndjson' -XPOST 'localhost:9200/_bulk?pretty' --data-binary @logs.jsonl
```
## Resources

- https://www.davincigroup.es/beats-elastic-ejemplo-filebeat/
- https://www.twosigma.com/articles/building-a-high-throughput-metrics-system-using-open-source-software/
