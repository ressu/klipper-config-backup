<!-- printerkeep: this file is not in the config folder. printerkeep writes it. -->
# pink-0

This branch holds the backups of the Klipper configuration of **pink-0**, made by
[printerkeep](https://github.com/ressu/printerkeep).

The files here are the printer's config folder (`printer_data/config`) as it was at the last backup.
This README is the one exception: printerkeep adds it here, and it is not on the printer. printerkeep
replaces any changes to it at the next backup.

Each backup is a commit, so the history of a file shows all its earlier versions.

## Restore this printer

For example after a new SD card:

1. Install Klipper and Moonraker, for example with KIAUH.
2. [Install printerkeep](https://github.com/ressu/printerkeep#install).
3. Run this on the printer:

   ```sh
   printerkeep restore --repository https://github.com/ressu/klipper-config-backup --printer-name pink-0
   ```

4. Restart Moonraker and Klipper.

## Shared files

This printer follows these files from the `shared` branch. It gets the changes that are made to
them there, and keeps its own changes. To see the status of each file, run `printerkeep status`
on the printer.

- `macros/filament.cfg`
- `macros/spoolman.cfg`
- `macros/reset.cfg`
- `macros/temperature.cfg`
