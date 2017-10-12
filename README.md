# Usage

```bash
docker run --rm -it -p 80:80 -e IP="127.0.0.1" celforyon/jupyter
```

# docker-compose.yml
```yaml
version: '3'
services:
	jupyter:
		container_name: jupyter
		image: celforyon/jupyter
		volumes:
		- ./jupyter:/jupyter
		environment:
		- IP="127.0.0.1"
```
