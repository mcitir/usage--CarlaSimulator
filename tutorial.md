### Client Creation
```python
client = carla.Client('localhost', 2000)
```

### World Connection
```python
world = client.get_world()

print(client.get_available_maps()) # get a list of available maps to change the current one.

world = client.load_world('Town01')

client.reload_world() # creates a new instance of the world with the same map. 
```
Every world object has an `id` or episode. Everytime the client calls for `load_world()` or `reload_world()` the previous one is destroyed. 


```python

```
