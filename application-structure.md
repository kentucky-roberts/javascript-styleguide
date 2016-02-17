# Application Structure


### Overall Guidelines


Have a near term view of implementation and a long term vision. In other words, start small but keep in mind on where the app is heading down the road. All of the app's code goes in a root folder named app. All content is 1 feature per file. Each controller, service, module, view is in its own file. All 3rd party vendor scripts are stored in another root folder and not in the app folder. I didn't write them and I don't want them cluttering my app (bower_components, scripts, lib).


### Application Structure LIFT Principal


* Structure your app such that you can Locate your code quickly, Identify the code at a glance, keep the Flattest structure you can, and Try to stay DRY. The structure should follow these 4 basic guidelines.


*Why LIFT?*: Provides a consistent structure that scales well, is modular, and makes it easier to increase developer efficiency by finding code quickly. Another way to check your app structure is to ask yourself: How quickly can you open and work in all of the related files for a feature?


### Layout


* Place components that define the overall layout of the application in a folder named layout. These may include a shell view and controller may act as the container for the app, navigation, menus, content areas, and other regions.



### Folders-by-Feature Structure

* Create folders named for the feature they represent. When a folder grows to contain more than 7 files, start to consider creating a folder for them. Your threshold may be different, so adjust as needed.


*Why?*: A developer can locate the code, identify what each file represents at a glance, the structure is flat as can be, and there is no repetitive nor redundant names.

*Why?*: The LIFT guidelines are all covered.

When I find my structure is not feeling comfortable, I go back and revisit these LIFT guidelines

1. Locating our code is easy
2. Identify code at a glance
3. Flat structure as long as we can
4. Try to stay DRY (Don't Repeat Yourself) or T-DRY




*Why?*: Helps reduce the app from becoming cluttered through organizing the content and keeping them aligned with the LIFT guidelines.

*Why?*: When there are a lot of files (10+) locating them is easier with a consistent folder structures and more difficult in flat structures.



**Recommended**
```
app/
    app.module.js
    app.config.js
    components/
        calendar.directive.js
        calendar.directive.html
        user-profile.directive.js
        user-profile.directive.html
    layout/
        shell.html
        shell.controller.js
        topnav.html
        topnav.controller.js
    people/
        attendees.html
        attendees.controller.js
        people.routes.js
        speakers.html
        speakers.controller.js
        speaker-detail.html
        speaker-detail.controller.js
    services/
        data.service.js
        localstorage.service.js
        logger.service.js
        spinner.service.js
    sessions/
        sessions.html
        sessions.controller.js
        sessions.routes.js
        session-detail.html
        session-detail.controller.js```


**Avoid:**
```
app/
    app.module.js
    app.config.js
    app.routes.js
    directives.js
    controllers/
        attendees.js
        session-detail.js
        sessions.js
        shell.js
        speakers.js
        speaker-detail.js
        topnav.js
    directives/
        calendar.directive.js
        calendar.directive.html
        user-profile.directive.js
        user-profile.directive.html
    services/
        dataservice.js
        localstorage.js
        logger.js
        spinner.js
    views/
        attendees.html
        session-detail.html
        sessions.html
        shell.html
        speakers.html
        speaker-detail.html
        topnav.html```





## Locate

* Make locating your code intuitive, simple and fast.


*Why?*: I find this to be super important for a project. If the team cannot find the files they need to work on quickly, they will not be able to work as efficiently as possible, and the structure needs to change. You may not know the file name or where its related files are, so putting them in the most intuitive locations and near each other saves a ton of time. A descriptive folder structure can help with this.