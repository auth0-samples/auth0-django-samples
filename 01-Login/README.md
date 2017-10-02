# Auth0 Python Web App Sample

This sample demonstrates how to add authentication to a Django web app using Auth0.

# Running the App

To run the sample, make sure you have `python`, `pip` installed.

Rename `.env.example` to `.env` and populate it with the client ID, domain, secret and audience for your
Auth0 app. If you are not implementing any API you can use `https://YOUR_DOMAIN.auth0.com/userinfo` as the audience.
Also, add the callback URL to the settings section of your Auth0 client.

Register `http://localhost:8000/complete/auth0` as `Allowed Callback URLs` and `http://localhost:8000`
as `Allowed Logout URLs` in your app settings.

Run `pip install -r requirements.txt` to install the dependencies, then run `python manage.py migrate` to migrate the
database and `python manage.py runserver 8000` to run the server.
The app will be served at [http://localhost:8000/](http://localhost:8000/).

# Running the App with Docker

In order to run the sample with [Docker](https://www.docker.com/) you need to add client ID, domain, secret and audience to `.env` file as explained [previously](#running-the-app)

Execute in command line `sh exec.sh` to build and run the docker image in Linux or `.\exec.ps1` to build and run the docker image 
in Windows.

## What is Auth0?

Auth0 helps you to:

* Add authentication with [multiple authentication sources](https://docs.auth0.com/identityproviders),
either social like **Google, Facebook, Microsoft Account, LinkedIn, GitHub, Twitter, Box, Salesforce, among others**,
or enterprise identity systems like **Windows Azure AD, Google Apps, Active Directory,
ADFS or any SAML Identity Provider**.
* Add authentication through more traditional 
**[username/password databases](https://docs.auth0.com/mysql-connection-tutorial)**.
* Add support for **[linking different user accounts](https://docs.auth0.com/link-accounts)**
with the same user.
* Support for generating signed [JSON Web Tokens](https://docs.auth0.com/jwt) to call your APIs and
**flow the user identity** securely.
* Analytics of how, when and where users are logging in.
* Pull data from other sources and add it to the user profile, through [JavaScript rules](https://docs.auth0.com/rules).

## Create a free account in Auth0

1. Go to [Auth0](https://auth0.com) and click Sign Up.
2. Use Google, GitHub or Microsoft Account to login.

## Issue Reporting

If you have found a bug or if you have a feature request, please report them at this repository issues section.
Please do not report security vulnerabilities on the public GitHub issue tracker.
The [Responsible Disclosure Program](https://auth0.com/whitehat) details the procedure for disclosing security issues.

## Author

[Auth0](https://auth0.com)

## License

This project is licensed under the MIT license. See the [LICENSE](LICENSE) file for more info.
