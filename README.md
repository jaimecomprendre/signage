# Signage feed

## Run

Put your media files in `media/<flux-name>/`.

Example:

```text
media/
  flux-1/
    image.jpg
    video.mp4
```

Start the stack:

```bash
docker compose up --build -d
```

## Windows

- Install Docker Desktop.
- Keep the project in a normal local folder, not a macOS-specific absolute path.
- Use `http://localhost:8000` on the same machine.
- Use `http://<your-ip>:8000` from another device.

## Feed output

Generated RSS files are written to `rss/`


file_url = f"{BASE_URL}/media/{urllib.parse.quote(folder_name)}/{urllib.parse.quote(filename)}"
