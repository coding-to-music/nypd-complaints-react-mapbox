# nypd-complaints-react-mapbox

# 🚀 Visualization of civilian complaints against New York City police officers as provided by ProPublica. 🚀

https://github.com/coding-to-music/nypd-complaints-react-mapbox

https://nypd-complaints-react-mapbox.vercel.app

From / By https://github.com/blahblahblah-/nypd-complaints

https://www.nypdcomplaints.com

## Environment variables:

```java
REACT_APP_MAPBOX_TOKEN=""
```

## GitHub

```java
git init
git add .
git remote remove origin
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:coding-to-music/nypd-complaints-react-mapbox.git
git push -u origin main
```

# NYPD Complaints

A frontend-only React app, providing visualization of civilian complaints against New York City police officers as provided by ProPublica.

Project was started with using [Create React App](https://create-react-app.dev/docs/getting-started/). Uses [Mapbox](https://www.mapbox.com) for maps, [Nivo](https://nivo.rocks/) for graphs, [Semantic UI React](https://react.semantic-ui.com/) for UI elements.

See it live at https://www.nypdcomplaints.com.

## Running locally

`````
$ brew install yarn
$ yarn install
`````

* Sign up for an account with [Mapbox](https://www.mapbox.com), get a token and add it to an `.env` file as `REACT_APP_MAPBOX_TOKEN`.

* Download datasets from [ProPublica](https://www.propublica.org/datastore/dataset/civilian-complaints-against-new-york-city-police-officers), drop CSV file into `data/`
* Download [NYC Police Precincts map data](https://data.cityofnewyork.us/Public-Safety/Police-Precincts/78dh-3ptz), drop geojson file as `src/data/precincts.json`

`````
$ node scripts/generateDataJson.js
$ yarn start
`````


