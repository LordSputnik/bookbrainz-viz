# BookBrainz data visualizations.

All charts are interactive. For plotly to work, there needs to be a `~/.plotly/.credentials` file present. See [here](https://plot.ly/python/getting-started/).

This connects to a PostgreSQL database whose options you can set by setting the environment variables `BBVIZ_USER`, `BBVIZ_PASSWORD`, `BBVIZ_HOST` and `BBVIZ_PORT`. The default is to connect to "postgres:admin@127.0.0.1:5432".
