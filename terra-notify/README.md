# terra-notify

Desktop notifications for Terra applications.

```bash
terra install terra-notify
```

```terra
use com.terra.notify;

func main(args: string[]) {
    notify.show("Reminders", "Time to stretch");
}
```

API:

- `notify.show(title, body)` — toast on the desktop
- `notify.is_available()` — `true` when the host can show toasts
