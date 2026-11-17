### Usage
```bash
LunarisRu_URL="https://github.com/andrey167/LunarisRu.git"
LunarisRu_DIR="$(pwd)/.LunarisRu_tmp"

rm -rf "$LunarisRu_DIR"
git clone --depth=1 "$LunarisRu_URL" "$LunarisRu_DIR" || {
    echo "ERROR: Failed to clone LunarisRu!"
    rm -rf "$LunarisRu_DIR"
    exit 1
}

cp -af "$LunarisRu_DIR/." "$(pwd)/"

rm -rf "$LunarisRu_DIR"
```
