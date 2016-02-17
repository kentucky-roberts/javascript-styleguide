# Application Structure


### Overall Guidelines


Have a near term view of implementation and a long term vision. In other words, start small but keep in mind on where the app is heading down the road. All of the app's code goes in a root folder named app. All content is 1 feature per file. Each controller, service, module, view is in its own file. All 3rd party vendor scripts are stored in another root folder and not in the app folder. I didn't write them and I don't want them cluttering my app (bower_components, scripts, lib).


### Layout


Place components that define the overall layout of the application in a folder named layout. These may include a shell view and controller may act as the container for the app, navigation, menus, content areas, and other regions.