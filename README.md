## Repo to jog my memory
<img src="https://image.ibb.co/bEF0B7/doggy.gif" alt="doggy" border="0">

### Why?
```TypeScript
- Not enough sleep or my memory is fading. This helps me keep track!
```

### Python | Pandas
```Python
df = pd.read_csv('<path/to/list')
print(df.head(5))
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

### SQL 
```
```

### Splunk SPL
```
```
