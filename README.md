# BookBrainz data visualizations

Setup instructions:

**NOTE**: You do not need to do this to just see the visualizations. Downloading
`bbviz.html` and opening it in your favorite web browser will show cached
visualizations that I made from the latest dump (`latest.tar`).

1. Clone this repository: `git clone https://github.com/eshansingh/bookbrainz-viz.git`
2. If you have anaconda/virtualenv installed, create a new environment for this.
3. Install [Jupyter Notebook](https://jupyter.org/install.html) if not present already.
4. Run `pip install -r requirements.txt`.
5. Create a new account on `plot.ly`, then visit [this page](https://plot.ly/settings/api) and use the
   username & API key from there to run this (in a Python REPL or in a script - you only need to do this once)

   ```python
   import plotly
   plotly.tools.set_credentials_file(username=YOUR_USERNAME, api_key=YOUR_API_KEY)
   ```
6. Make sure you have a PostgreSQL database running on `127.0.0.1:5432` with username `postgres` and password `admin`. Or,
   change the environment variables `BBVIZ_HOST`, `BBVIZ_PORT`, `BBVIZ_USER` and `BBVIZ_PASSWORD` to your values.
7. Run `jupyter notebook bbviz.ipynb`.
8. ![**PROFIT!**](https://proxy.duckduckgo.com/iu/?u=https%3A%2F%2Fmedia.giphy.com%2Fmedia%2Fg8S1ntWFumtmE%2Fgiphy.gif&f=1)
