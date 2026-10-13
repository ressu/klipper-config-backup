<!-- printerkeep: this file is not in the config folder. printerkeep writes it. -->
# bluev2

This branch has the backups of the Klipper configuration of **bluev2**, made by
[printerkeep](https://github.com/ressu/printerkeep). The files of this branch are the files of the config folder
(`printer_data/config`) of the printer. Only this README.md is not in the config folder:
printerkeep writes it, and replaces changes to it.

Each backup is a commit. To see an older version of a file, open the history of the file.

## Restore the printer

For example after a new SD card:

1. Install Klipper and Moonraker (for example with KIAUH).
2. Install printerkeep: https://github.com/ressu/printerkeep#install
3. On the printer, run:

   ```sh
   printerkeep restore https://github.com/ressu/klipper-config-backup --printer-name bluev2
   ```

4. Restart Moonraker and Klipper.
