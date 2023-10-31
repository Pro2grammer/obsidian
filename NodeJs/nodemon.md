it refreshes server on save
npm install nodemon -D

we use -D here to use it as a devDepedency ie will not be used in production as it is out and only while developing

also in packaage .json we can in script use
"scripts": {
"start":"node app.js"
}

so if i type "npm start" it runs "node app.js" command

but with others you need to use "npm run and command"
"dev":"nodemon app.js"
use
"npm run dev"

press ctrl+c to stop server


TO uninstall package
npm uninstall packagename



