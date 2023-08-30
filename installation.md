## Launch Carla with option
- Go to folder `cd /opt/carla-simulator` if you install via debian package
- run sh script `./CarlaUE4.sh` without an option 

| Feature  | Option Code |
| :------------- | :------------- |
|Run by using Nvidia Card | `./CarlaUE4.sh -prefernvidia`|
|Low graphical details | `./CarlaUE4.sh -quality-level=Low`|
|Listen specific port |  `./CarlaUE4.sh -carla-rpc-port=N` # Listen for client connections at port `N`. Streaming port is set to `N+1` by default.|
|Specify special port for sensor data streaming| `./CarlaUE4.sh -carla-streaming-port=N` # second port will be `N+1`, use N=0 for random port|

## Check that Python libraries are defined correctly

```bash
export PYTHONPATH=$PYTHONPATH:<path/to/carla/>/PythonAPI/carla/dist/<your_egg_file>
# Check if CARLA can now be found
python3 -c 'import carla;print("Success")'
```
