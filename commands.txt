ng new mono-workspace --createApplication="false"
cd mono-workspace
ng g application host-app --routing --style=scss
ng g application mfe-app --routing --style=scss
npm i webpack webpack-cli --save-dev
ng add @angular-architects/module-federation --project host-app --port 4200
ng add @angular-architects/module-federation --project mfe-app --port 4300
