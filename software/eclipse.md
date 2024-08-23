# Eclipse

## Adding Eclipse to Ubuntu Start Menu

Within the **~/.local/share/applications** directory, create a file with any name, but ending in ".desktop"

It should look similar to the example below:

```bash
# Filename: _home_michael_eclipse_jee-2024-06_eclipse_.desktop
[Desktop Entry]
Name=Eclipse IDE
Exec= env GDK_BACKEND=x11 /home/michael/eclipse/jee-2024-06/eclipse/eclipse %u
NoDisplay=true
Type=Application
MimeType=x-scheme-handler/eclipse+command;x-scheme-handler/eclipse+mpc;
```

Exec should have a path pointing to the directory where the eclipse binary resides.