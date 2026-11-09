<!-- printerkeep: this file is not in the config folder. printerkeep writes it. -->
# pink-0

The Klipper configuration of **pink-0**, backed up by [printerkeep](https://github.com/ressu/printerkeep). Each backup is a
commit, so the history of a file shows all its earlier versions.

## What's here

- **The printer's config folder** (`printer_data/config`), as it was at the last backup.
- **This README**, the one exception: printerkeep adds it here, and it isn't on the printer.
  printerkeep replaces any changes to it at the next backup.

## Shared files

This printer follows these files from the [`shared` branch](https://github.com/ressu/klipper-config-backup/tree/shared). It gets the changes that are made to them there,
and keeps its own changes. The README of `shared` lists the other printers that follow shared
files.

| File | Shared version |
| --- | --- |
| [`macros/filament.cfg`](macros/filament.cfg) | [on shared](https://github.com/ressu/klipper-config-backup/blob/shared/macros/filament.cfg) |
| [`macros/spoolman.cfg`](macros/spoolman.cfg) | [on shared](https://github.com/ressu/klipper-config-backup/blob/shared/macros/spoolman.cfg) |
| [`macros/reset.cfg`](macros/reset.cfg) | [on shared](https://github.com/ressu/klipper-config-backup/blob/shared/macros/reset.cfg) |
| [`macros/temperature.cfg`](macros/temperature.cfg) | [on shared](https://github.com/ressu/klipper-config-backup/blob/shared/macros/temperature.cfg) |

To see the status of each file, run this on the printer:

```sh
printerkeep status
```

## Go back to an earlier version

To bring back a file as it was at some time, run this on the printer:

```sh
printerkeep restore "<file>" --at "2 days ago"
```

Without `--at`, printerkeep lists the earlier versions of the file, and you pick one.

## Restore this printer

For example after a new SD card:

1. Install Klipper and Moonraker, for example with KIAUH.
2. [Install printerkeep](https://github.com/ressu/printerkeep#install).
3. Run this on the printer:

   ```sh
   printerkeep restore --repository https://github.com/ressu/klipper-config-backup --printer-name pink-0
   ```

4. Restart Moonraker and Klipper.
