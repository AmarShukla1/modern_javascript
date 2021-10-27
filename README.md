previously to include an outside library we had to include its js file in the html of our code.
but that was not optimal as the dependencies versions change and we won't know if that happened or not
we want to have a package manager like thing which could do such things
npm,yarn are such package managers.npm is currently the most popular.
So that's that one uses package manager for their own ease.

for using packages in the nodejs you just have to write require beacuse npm is for that purpose.
for using packages to use the code in them in browser one has to find the required file and then include it by manually typing,because the browser has not access to file system so it cannot do that.

In this regard webpack helps us it is there in the npm though so some people get confused that npm is for server side why is it helping in frontend.webpack bundles all the code that is required you just have to specify your input and output in the config file of webpack.Also you have to use require ot import which library you are trying to use.

With that said npx webpack will take our script at src/index.js as the entry point, and will generate dist/main.js as the output. The npx command, which ships with Node 8.2/npm 5.2.0 or higher, runs the webpack binary (./node_modules/.bin/webpack) of the webpack package.if we run in our shell the command to run that binary will do the same thing as npx webpack does.

webpack gives this important functionality.One can use external libraries in the frontend that's how react is being done.It comes with webpack and babel being configured.babel is a transpiler it converts new code into old because all the browsers are not fast enough to adopt all the latest standards so that's that.One can use task runner,dev server and other things by configuring webpack.

Behind the scenes, webpack actually "transpiles" the code so that older browsers can also run it.


So all the technical jargon has been cleared as of now I understand the basic things of these why are they being used and what purpose they serve will dive deep in this whenever required in project.