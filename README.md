# nmma_db
database and API for the NMMA framework

## Quick Start
Setup your config file: cp config.defaults.yaml config.yaml

Setup your postgres options:

sudo -i -u postgres

Add options to pg_hba.conf:

host nmma nmma ::1/128 trust
host nmma_test nmma ::1/128 trust

To initialize the database: python nmma_db/models.py --init_db

To enable API interaction: python nmma_db/api.py
