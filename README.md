# sys_perf_check_tool
## Running the tool
### Start the server_end_script
```
# requires a components.json file
# run the below script on the server where you are hosting your project and want to measure its performance
python3 server_end_script.py
```
### Running cliend_end_script
```
# install docker if not present
```
#### Build the docker container
```
$ docker build -t <image_name>
```

#### Run the script using the docker container
```
$ docker run --rm -p 5500:5500 -v $(pwd):/app <image_name> python3 client_end_script.py -l 50 -u 60 -s 10 -t 30
```