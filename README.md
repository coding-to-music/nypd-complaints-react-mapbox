# nypd-complaints-react-mapbox

# 🚀 Visualization of civilian complaints against New York City police officers as provided by ProPublica. 🚀

https://github.com/coding-to-music/nypd-complaints-react-mapbox

https://nypd-complaints-react-mapbox.vercel.app (not set up)

From / By https://github.com/blahblahblah-/nypd-complaints

https://www.nypdcomplaints.com

https://www.propublica.org/datastore/dataset/civilian-complaints-against-new-york-city-police-officers

33,358 rows of data

https://medium.com/@_blahblahblah/visualizing-the-propublica-nypd-files-41c0ccc8a156

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
Failed to compile.

Attempted import error: 'Responsive' is not exported from 'semantic-ui-react' (imported as 'Responsive').
ERROR in ./src/App.jsx 72:38-48
export 'Responsive' (imported as 'Responsive') was not found in 'semantic-ui-react'
```

## docs(Responsive): deprecate

This PR marks Responsive as deprecated, we will remove it in the next major release, i.e. 2.0.0.

https://github.com/Semantic-Org/Semantic-UI-React/pull/4008

https://www.npmjs.com/package/semantic-ui-react?activeTab=versions

Previous version was 1.3.1

```
npm install semantic-ui-react@1.3.1 --legacy-peer-deps
```

## Still getting errors

```
  "dependencies": {
    "@nivo/bar": "^0.80.0",
    "@testing-library/jest-dom": "^5.16.5",
    "@testing-library/react": "^13.4.0",
    "@testing-library/user-event": "^14.4.3",
    "mapbox-gl": "^2.12.0",
    "node-sass": "^8.0.0",
    "react": "^18.2.0",
    "react-datepicker": "^4.8.0",
    "react-dom": "^18.2.0",
    "react-helmet": "^6.1.0",
    "react-router-dom": "^6.6.2",
    "react-scripts": "5.0.1",
    "semantic-ui-react": "^1.3.1"
  },
```

## Errors

```
Failed to compile.

Attempted import error: 'Switch' is not exported from 'react-router-dom' (imported as 'Switch').
ERROR in ./src/App.jsx 157:53-59
export 'Switch' (imported as 'Switch') was not found in 'react-router-dom' (possible exports: AbortedDeferredError, Await, BrowserRouter, Form, HashRouter, Link, MemoryRouter, NavLink, Navigate, NavigationType, Outlet, Route, Router, RouterProvider, Routes, ScrollRestoration, UNSAFE_DataRouterContext, UNSAFE_DataRouterStateContext, UNSAFE_LocationContext, UNSAFE_NavigationContext, UNSAFE_RouteContext, UNSAFE_enhanceManualRouteObjects, UNSAFE_useScrollRestoration, createBrowserRouter, createHashRouter, createMemoryRouter, createPath, createRoutesFromChildren, createRoutesFromElements, createSearchParams, defer, generatePath, isRouteErrorResponse, json, matchPath, matchRoutes, parsePath, redirect, renderMatches, resolvePath, unstable_HistoryRouter, useActionData, useAsyncError, useAsyncValue, useBeforeUnload, useFetcher, useFetchers, useFormAction, useHref, useInRouterContext, useLinkClickHandler, useLoaderData, useLocation, useMatch, useMatches, useNavigate, useNavigation, useNavigationType, useOutlet, useOutletContext, useParams, useResolvedPath, useRevalidator, useRouteError, useRouteLoaderData, useRoutes, useSearchParams, useSubmit)

ERROR in ./src/App.jsx 201:39-47
export 'Redirect' (imported as 'Redirect') was not found in 'react-router-dom' (possible exports: AbortedDeferredError, Await, BrowserRouter, Form, HashRouter, Link, MemoryRouter, NavLink, Navigate, NavigationType, Outlet, Route, Router, RouterProvider, Routes, ScrollRestoration, UNSAFE_DataRouterContext, UNSAFE_DataRouterStateContext, UNSAFE_LocationContext, UNSAFE_NavigationContext, UNSAFE_RouteContext, UNSAFE_enhanceManualRouteObjects, UNSAFE_useScrollRestoration, createBrowserRouter, createHashRouter, createMemoryRouter, createPath, createRoutesFromChildren, createRoutesFromElements, createSearchParams, defer, generatePath, isRouteErrorResponse, json, matchPath, matchRoutes, parsePath, redirect, renderMatches, resolvePath, unstable_HistoryRouter, useActionData, useAsyncError, useAsyncValue, useBeforeUnload, useFetcher, useFetchers, useFormAction, useHref, useInRouterContext, useLinkClickHandler, useLoaderData, useLocation, useMatch, useMatches, useNavigate, useNavigation, useNavigationType, useOutlet, useOutletContext, useParams, useResolvedPath, useRevalidator, useRouteError, useRouteLoaderData, useRoutes, useSearchParams, useSubmit)

ERROR in ./node_modules/@nivo/annotations/dist/nivo-annotations.es.js 5:0-184
Module not found: Error: Can't resolve '@nivo/core' in '/mnt/volume_nyc1_01/nypd-complaints-react-mapbox/node_modules/@nivo/annotations/dist'

ERROR in ./node_modules/@nivo/axes/dist/nivo-axes.es.js 4:0-112
Module not found: Error: Can't resolve '@nivo/core' in '/mnt/volume_nyc1_01/nypd-complaints-react-mapbox/node_modules/@nivo/axes/dist'

ERROR in ./node_modules/@nivo/bar/dist/nivo-bar.es.js 5:0-301
Module not found: Error: Can't resolve '@nivo/core' in '/mnt/volume_nyc1_01/nypd-complaints-react-mapbox/node_modules/@nivo/bar/dist'

ERROR in ./node_modules/@nivo/legends/dist/nivo-legends.es.js 3:0-90
Module not found: Error: Can't resolve '@nivo/core' in '/mnt/volume_nyc1_01/nypd-complaints-react-mapbox/node_modules/@nivo/legends/dist'

ERROR in ./node_modules/@nivo/tooltip/dist/nivo-tooltip.es.js 3:0-106
Module not found: Error: Can't resolve '@nivo/core' in '/mnt/volume_nyc1_01/nypd-complaints-react-mapbox/node_modules/@nivo/tooltip/dist'

webpack compiled with 7 errors
```

## Another install needed: @nivo/core

```
npm i @nivo/core --legacy-peer-deps
```

## npm run start

```

Attempted import error: 'Switch' is not exported from 'react-router-dom' (imported as 'Switch').
ERROR in ./src/App.jsx 157:53-59
export 'Switch' (imported as 'Switch') was not found in 'react-router-dom' (possible exports: AbortedDeferredError, Await, BrowserRouter, Form, HashRouter, Link, MemoryRouter, NavLink, Navigate, NavigationType, Outlet, Route, Router, RouterProvider, Routes, ScrollRestoration, UNSAFE_DataRouterContext, UNSAFE_DataRouterStateContext, UNSAFE_LocationContext, UNSAFE_NavigationContext, UNSAFE_RouteContext, UNSAFE_enhanceManualRouteObjects, UNSAFE_useScrollRestoration, createBrowserRouter, createHashRouter, createMemoryRouter, createPath, createRoutesFromChildren, createRoutesFromElements, createSearchParams, defer, generatePath, isRouteErrorResponse, json, matchPath, matchRoutes, parsePath, redirect, renderMatches, resolvePath, unstable_HistoryRouter, useActionData, useAsyncError, useAsyncValue, useBeforeUnload, useFetcher, useFetchers, useFormAction, useHref, useInRouterContext, useLinkClickHandler, useLoaderData, useLocation, useMatch, useMatches, useNavigate, useNavigation, useNavigationType, useOutlet, useOutletContext, useParams, useResolvedPath, useRevalidator, useRouteError, useRouteLoaderData, useRoutes, useSearchParams, useSubmit)

ERROR in ./src/App.jsx 201:39-47
export 'Redirect' (imported as 'Redirect') was not found in 'react-router-dom' (possible exports: AbortedDeferredError, Await, BrowserRouter, Form, HashRouter, Link, MemoryRouter, NavLink, Navigate, NavigationType, Outlet, Route, Router, RouterProvider, Routes, ScrollRestoration, UNSAFE_DataRouterContext, UNSAFE_DataRouterStateContext, UNSAFE_LocationContext, UNSAFE_NavigationContext, UNSAFE_RouteContext, UNSAFE_enhanceManualRouteObjects, UNSAFE_useScrollRestoration, createBrowserRouter, createHashRouter, createMemoryRouter, createPath, createRoutesFromChildren, createRoutesFromElements, createSearchParams, defer, generatePath, isRouteErrorResponse, json, matchPath, matchRoutes, parsePath, redirect, renderMatches, resolvePath, unstable_HistoryRouter, useActionData, useAsyncError, useAsyncValue, useBeforeUnload, useFetcher, useFetchers, useFormAction, useHref, useInRouterContext, useLinkClickHandler, useLoaderData, useLocation, useMatch, useMatches, useNavigate, useNavigation, useNavigationType, useOutlet, useOutletContext, useParams, useResolvedPath, useRevalidator, useRouteError, useRouteLoaderData, useRoutes, useSearchParams, useSubmit)

webpack compiled with 2 errors
```

## Install earlier version of react-router-dom

```
npm install react-router-dom@5.3.4 --legacy-peer-deps
```

## Need to create file

Downloaded File is named: allegations_202007271729.csv

Needs to be called allegations.json and be stored in ./src/data

Then run npm run seed and the json file will be created from the .csv file

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

## Seed the json file with data from the csv

```
npm run seed
```

Output

```
> nypd-complaints-react-mapbox@0.1.0 seed
> node scripts/generateDataJson.js

5000 rows processed
10000 rows processed
15000 rows processed
20000 rows processed
25000 rows processed
30000 rows processed
33359 rows processed
success
The file has been saved!
```
