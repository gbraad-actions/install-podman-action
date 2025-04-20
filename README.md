Install Podman on Windows
=========================


Install podman on windows runners

```yaml
    runs-on: windows-latest
    steps:
      - uses: gbraad-actions/install-podman-action@main
      - name: Initialize Podman machine
        run: |
          podman machine init
          podman machine start
          podman run hello-world
```
