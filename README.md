<!-- printerkeep: this file is not in the config folder. printerkeep writes it. -->
# Printer configuration

This repository holds the Klipper configuration of several printers, made by
[printerkeep](https://github.com/ressu/printerkeep).

- **Each printer has its own branch,** named after the printer. Select it in the branch list of the
  repository. It holds the printer's config folder, and a README with the steps to restore it.
- **This branch, `shared`, holds the shared files.** A printer that follows a shared file gets the
  changes that are made to it here, and keeps its own changes. To see the status of each file, run
  `printerkeep status` on the printer.

## Restore a printer

Install Klipper, Moonraker and [printerkeep](https://github.com/ressu/printerkeep#install). Then run this on the printer:

```sh
printerkeep restore --repository https://github.com/ressu/klipper-config-backup --printer-name <printer name>
```

You can edit this README. Delete its first line (a hidden comment) first: printerkeep then leaves it
as it is.
