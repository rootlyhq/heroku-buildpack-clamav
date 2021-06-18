# heroku-buildpack-clamav
A heroku buildpack for setting up [ClamAv](https://www.clamav.net/)

## Usage

1. Add the following buildpacks to your heroku app:
  + `https://github.com/heroku/heroku-buildpack-apt`
  + `https://github.com/GugahBrz/heroku-buildpack-clamav`
2. Add an `Aptfile` in your project root with the following dependences:
  + clamav
  + clamav-daemon
  + clamav-freshclam
3. Setup your `clamd.conf` and `freshclam.conf` files in the `config/clamav` directory
4. Trigger a new deployment and that’s it.
