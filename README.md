# Dedupe Calcurse Appointments

If you attempt to import a .ics file into [calcurse](https://calcurse.org/), it will [introduce duplicate events](https://bugs.calcurse.org/frs/24/).

This script attempts to remove those duplicates.

## Usage

After importing a calender using `calcurse -i calender.ics`, run

```
    ./post_import_dedepe
```

If your calendar is not in `~/.calcurse/`, you can set the correct directory using the environment variable `CALCURSE_DIR`.

```
    CALCURSE_DIR="${HOME}/dropbox/.calcurse" ./post_import_dedepe
```

