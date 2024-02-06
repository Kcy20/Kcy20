## Repo to jog my memory
<img src="https://image.ibb.co/bEF0B7/doggy.gif" alt="doggy" border="0">

### Why?
```TypeScript
- Not enough sleep or my memory is fading. This helps me keep track!
```

### Projects that are WIP
```TypeScript
- Working on a Python|Flask|MongoDB project that usings the nba_api package 
    - Which will be filtered to pull season data from the current season (https://pypi.org/project/nba_api/)
- Goal is to display stat data (graphs, plots, tables) 
    - In a way that helps sports prop bettors or enthusiasts look at the full picture of any players stats
```

### Python | Pandas
```Python
df = pd.read_csv('<path/to/list')
print('\nData looks like this:\n', df.head(5))
## https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#timeseries-offset-aliases
current_time = pd.Timestamp.now(tz='US/Central').floor('s')
alert_time = pd.Timestamp.now(tz='US/Central') - pd.Timedelta('10 hours')
df['copy2_newcolumn'] = pd.to_datetime(slist['copy1'], unit='ms').dt.tz_localize('US/Central').dt.tz_convert(None)
df['foo'] = df.apply(lambda row: row['f'] + row['o'] + row['o'], axis=1)
df.drop(["f", "o", "o"], axis=1, inplace=True) # drop columns
```

### PyMongo
```Python
client = pymongo.MongoClient(url)
db = client.<dbName>> 
collection = db.<collName> 
requesting = []

with open(r"../files/files.json") as f:
    for jsonObj in f:
        myDict = json.loads(jsonObj)
        requesting.append(InsertOne(myDict))

result = collection.bulk_write(requesting)
client.close()
```

### Unix | Shell Bash | 
```Shell

```

### DevOps | Terraform | Ansible 
```TypeScript
terraform init
terraform fmt
terraform validate
terraform plan -out=terraform.plan
terraform apply terraform.plan
terraform show
terraform state list
terraform destory
```

### Splunk SPL
```TypeScript
| tstats count where index=* sourcetype=* by _time span=1h index | timechart span=1h sum(count) by index limit=0 usenull=false
```
