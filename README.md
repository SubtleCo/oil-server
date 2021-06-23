# oil-server
The Python/Django API counterpart to the Oil React app.

### [Visit the deployed site](https://oil-client.netlify.app)

For detailed instructions, samples, and information, please visit the client repository below.

### [Client](https://github.com/SubtleCo/Oil)

### Instructions for Use - Installing the server
1. Make a copy of the `.env.example` file in the directory `Oil/server/oil/oil` and remove the .example extension.
2. Acquire an secret key for Django by running the following command:
`python -c 'from django.core.management.utils import get_random_secret_key; print(get_random_secret_key())'`
3. Insert the resulting secret key into your new `.env` file
4. Change directories to `Oil/server/oil` and star a new environment shell by running the command `pipenv shell`
5. In `Oil/server/oil` seed the database with the command `./seed.sh`. If you get a permissions error, run `sudo ./seed.sh` and enter your machine user password when prompted
6. Run the server with the command `python3 manage.py runserver` (or `python` if you prefer)
