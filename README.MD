semgrep plugin for static analysis

Build the Docker image
```bash
docker build -t semgrep-plugin:arm64 -f Dockerfile.linux.arm64 .
```

Testing
```bash
docker run --rm -e \  
-e PLUGIN_SRC_ROOT_DIR=migrate \
plugins/semgrep-runner
```