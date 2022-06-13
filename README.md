<img src="https://user-images.githubusercontent.com/7164864/172889064-79428a48-07f8-4de0-ba70-c5cf101f3411.png" width="200"></img>

# Streamlit demo: 🌀 The Snowflake Usage Insights app

This app provides insights on a demo Snowflake account usage.

It was made using :balloon: [Streamlit](https://www.streamlit.io) and the :snowflake: [Snowflake Python connector](https://github.com/snowflakedb/snowflake-connector-python)!

### Can I use this app with my own Snowflake account?

This demo app currently only supports basic username / password authentication
to connect to your Snowflake account. For security purposes, we recommend cloning this app and running it **locally** instead of on Streamlit Cloud. If you're interested, head over to the next section!

### Run this app locally
Follow these steps:

1. **Set up dependencies.** Get [Pipenv](https://pipenv-fork.readthedocs.io/en/latest/install.html#pragmatic-installation-of-pipenv),
clone/fork this repository and within the directory, run:
```
pipenv clean && pipenv install --python 3.9
```

2. **Set up credentials.** Create a file `.streamlit/secrets.toml` and fill in your Snowflake account
credentials. The file should look like this:
```
[sf_usage_app]
user = "..."
account = "..."
password = "..."
```

3. **Run the app locally.** Simply run:
```
pipenv run streamlit run Home.py
```

🎊 Your browser should now be opened with the Streamlit app running locally!

### Contribute

Feel free to contribute! Simply make sure to:
1. Install development dependencies `pipenv install --python 3.9 --dev`
2. Set up pre-commit hooks `pipenv run pre-commit install`

### Questions? Comments?

Please ask in the [Streamlit community](https://discuss.streamlit.io).
