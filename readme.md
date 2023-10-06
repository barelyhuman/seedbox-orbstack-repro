# seedbox-orbstack-repro

The problem involves Sonarr blocking / freezing docker from taking commands.

The following repro sets up a basic seedbox setup for it.

## Launch Instructions

Most of the configuration is already in place. Just run `docker compose up`

```sh
$ docker compose up -d
```

- Open up `localhost:8989` in your browser, open the added Anime title
  `Eminence in the Shadow` and click on `Search Monitored` , wait for it to
  start downloading the episodes which can be monitored on the `Activity`
  Section from the Sidebar.
- Let this run for about 20-30 minutes and you'll then see that none of the
  `docker` commands run anymore and just timeout
