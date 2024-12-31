## Additional notes for those trying the streamlit/grafana out

1) The following packages are required when you run some of .py scripts

```
pip install psycopg2-binary python-dotenv
pip install pgcli
```
command to execute:
```
export POSTGRES_HOST="localhost"
```
Then run `python prep.py` to prepare for the data.
To check data exists with pgcli:
```
pgcli -h localhost -U your_username -d course_assistant -W
```

2) To download the phi3 model to the container
```
docker-compose up -d
docker-compose exec ollama ollama pull phi3
```