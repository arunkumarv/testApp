# TestApp

## Environment
Angular CLI: 10.1.7\
Node: 12.14.1

## What I did
- I created a folder test and created `ng new testApp` in test folder with routing as true & style CSS. 
- Created another folder test/static/client. Treat static as static folder of the server. 
- my relative path of app is static/client
So Now the folder structure is
```
test/testApp - is angular app
test/static/client - is just a folder
```
- take a look at line 16 & 17 of angular.json
```
"outputPath": "../static/client/",
"baseHref": "/client/",
```
- If environment is same clone the project. Otherwise create a project and replace contents of src/ with this src/. 
_Note: Updates are on app-router.module.ts and app.component.ts. Created three components home, about, contact_
- `ng serve` and go to `http://localhost:4200/client`
- `ng build --prod`
- Take a look at `static/client`.
- At static/ folder run python3.7 -m http.server and go to `http://localhost:8000/client`. Try the links.

## What we did is:
- Assume that static/ is the static folder of the project.
- client/ is the relative path of app at static path.
- Configured angular.json for relative paths.
- configured routes at app-routing.module.ts