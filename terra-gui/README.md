# terra-gui

Desktop UI toolkit for Terra. Install with:

```bash
terra install terra-gui
# or
terra install com.terra.ui
```

## Quick start

```terra
use com.terra.ui;
use com.terra.json;

css "styles/app.css";

func view(state: string) -> any {
    return ui.page("My App", "raw", ui.col([
        ui.h1("Hello"),
        ui.button("Click", "click")
    ]), state);
}

func main(args: string[]) {
    ui.desktop("My App", 900, 640, "view");
}
```

Prefer function layouts (`ui.col`, `ui.row`, `ui.button`) over JSX. Use `theme: "raw"` and your own CSS for a native desktop look.
