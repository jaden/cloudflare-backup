# cloudflare-backup

Simple tool for backing up your CloudFlare hosted DNS records

## Configuration

In Cloudflare, create an API token with Zone.Zone, Zone.DNS on All Zones (read-only)

Add this token value to a `.env` file with a key of `CF_TOKEN`.

An API token is preferred to a key so you can limit the access to read-only on a subset of the account.

## Installation

Run `npm install`

## Usage

`npm start`

All of the DNS records for all of your zones will be dumped in a BIND compatible format.
