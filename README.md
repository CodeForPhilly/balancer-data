# Balancer Data
This repo is a hugo site that generates a JSON api.  You add data by adding markdown files, and github pages hosts the API.

## Github pages
The generated site and api can be seen at https://codeforphilly.github.io/balancer-data/

# API

## Medication List
You can see the medication list json at https://codeforphilly.github.io/balancer-data/api/medications/index.json

## Symptoms list
The list of symptoms is at https://codeforphilly.github.io/balancer-data/api/symptoms/index.json


# Adding Data
To add data you can use the hugo command line tool to create a new file for you using the archetype template.  Or you can create or edit an existing markdown file.

## Using the hugo command line tool
If you are on a mac you can use [Homebrew](https://brew.sh) to install [Hugo](https://gethugo.io) by running `brew install hugo`.

Once you have hugo, in this project's working directory you can create a new medication by running

```sh
hugo new api/medications/med-name.md
```

This will create a markdown file in `content/api/medications/med-name.md`.  If you have no other information to add, then you can commit and push up the file and it will be added to the list.

## Testing locally
To run the hugo server locally, run

```sh
hugo serve
```

This will run the hugo server locally, and you can navigate to `http://localhost:1313/balancer-data/` to see the site and API running.
