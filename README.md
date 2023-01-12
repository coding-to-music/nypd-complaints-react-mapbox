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

## Update/upgrade NPM dependancies

```
[====================] 14/14 100%

 @nivo/bar                     ^0.62.0  →  ^0.80.0
 @testing-library/jest-dom      ^4.2.4  →  ^5.16.5
 @testing-library/react         ^9.3.2  →  ^13.4.0
 @testing-library/user-event    ^7.1.2  →  ^14.4.3
 mapbox-gl                     ^1.11.1  →  ^2.12.0
 node-sass                     ^4.14.1  →   ^8.0.0
 react                        ^16.13.1  →  ^18.2.0
 react-datepicker               ^3.1.3  →   ^4.8.0
 react-dom                    ^16.13.1  →  ^18.2.0
 react-router-dom               ^5.2.0  →   ^6.6.2
 react-scripts                   3.4.1  →    5.0.1
 semantic-ui-react              ^1.0.0  →   ^2.1.4

Run ncu -u to upgrade package.json
```

# NPM run start gives errors

```
Compiled with problems:X

ERROR in ./src/App.jsx 21:4-37

Module not found: Error: Can't resolve './data/allegations.json' in '/mnt/volume_nyc1_01/nypd-complaints-react-mapbox/src'


ERROR in ./src/App.jsx 72:38-48

export 'Responsive' (imported as 'Responsive') was not found in 'semantic-ui-react' (possible exports: Accordion, AccordionAccordion, AccordionContent, AccordionPanel, AccordionTitle, Advertisement, Breadcrumb,
```

## Need to create file

Downloaded File is named: allegations_202007271729.csv

Needs to be called allegations.json and be stored in ./src/data

# NYPD Complaints

A frontend-only React app, providing visualization of civilian complaints against New York City police officers as provided by ProPublica.

Project was started with using [Create React App](https://create-react-app.dev/docs/getting-started/). Uses [Mapbox](https://www.mapbox.com) for maps, [Nivo](https://nivo.rocks/) for graphs, [Semantic UI React](https://react.semantic-ui.com/) for UI elements.

See it live at https://www.nypdcomplaints.com.

## Running locally

```
$ brew install yarn
$ yarn install
```

- Sign up for an account with [Mapbox](https://www.mapbox.com), get a token and add it to an `.env` file as `REACT_APP_MAPBOX_TOKEN`.

- Download datasets from [ProPublica](https://www.propublica.org/datastore/dataset/civilian-complaints-against-new-york-city-police-officers), drop CSV file into `data/`
- Download [NYC Police Precincts map data](https://data.cityofnewyork.us/Public-Safety/Police-Precincts/78dh-3ptz), drop geojson file as `src/data/precincts.json`

```
$ node scripts/generateDataJson.js
$ yarn start
```
