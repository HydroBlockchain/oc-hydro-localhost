# oc-hydro-localhost

A working October CMS installation for testing the Hydro Raindrop plugin.

## Installation

- Check out this repository and `cd` to root.
- `cp .env.example .env`
- Create MySQL database `oc-hydro-localhost` (use `utf8mb4` encoding for the database).
- Update the database parameters in `.env`
- `composer update`
- `php artisan theme:use hydroraindropdemo` (set active theme).
- Navigate to `https://hostname/backend`, log in with user `admin` and password `admin`.

## Reset Hydro Raindrop plugin

This will re-create the required tables.

`php artisan plugin:refresh HydroCommunity.Raindrop` 

This will remove all vendor packages and re-install all packages.

`./update.sh`
