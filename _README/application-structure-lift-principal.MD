### Application Structure LIFT Principal

Structure your app such that you can Locate your code quickly, Identify the code at a glance, keep the Flattest structure you can, and Try to stay DRY. The structure should follow these 4 basic guidelines.

Why LIFT?: Provides a consistent structure that scales well, is modular, and makes it easier to increase developer efficiency by finding code quickly. Another way to check your app structure is to ask yourself: How quickly can you open and work in all of the related files for a feature?

When I find my structure is not feeling comfortable, I go back and revisit these LIFT guidelines

<ul>
<li>Locating our code is easy</li>
<li>Identify code at a glance</li>
<li>Flat structure as long as we can</li>
<li>Try to stay DRY (Don’t Repeat Yourself) or T-DRY</li>
</ul>

### Locate

Make locating your code intuitive, simple and fast.

Why?: I find this to be super important for a project. If the team cannot find the files they need to work on quickly, they will not be able to work as efficiently as possible, and the structure needs to change. You may not know the file name or where its related files are, so putting them in the most intuitive locations and near each other saves a ton of time. A descriptive folder structure can help with this.

### Identify

When you look at a file you should instantly know what it contains and represents.

Why?: You spend less time hunting and pecking for code, and become more efficient. If this means you want longer file names, then so be it. Be descriptive with file names and keeping the contents of the file to exactly 1 component. Avoid files with multiple controllers, multiple services, or a mixture. There are deviations of the 1 per file rule when I have a set of very small features that are all related to each other, they are still easily identifiable.


### Flat

Keep a flat folder structure as long as possible. When you get to 7+ files, begin considering separation.

Why?: Nobody wants to search 7 levels of folders to find a file. Think about menus on web sites … anything deeper than 2 should take serious consideration. In a folder structure there is no hard and fast number rule, but when a folder has 7-10 files, that may be time to create subfolders. Base it on your comfort level. Use a flatter structure until there is an obvious value (to help the rest of LIFT) in creating a new folder.



### T-DRY (Try to Stick to DRY)

Be DRY, but don't go nuts and sacrifice readability.

Why?: Being DRY is important, but not crucial if it sacrifices the others in LIFT, which is why I call it T-DRY. I don’t want to type session-view.html for a view because, well, it’s obviously a view. If it is not obvious or by convention, then I name it.




### Overall Guidelines

Have a near term view of implementation and a long term vision. In other words, start small but keep in mind on where the app is heading down the road. All of the app's code goes in a root folder named app. All content is 1 feature per file. Each controller, service, module, view is in its own file. All 3rd party vendor scripts are stored in another root folder and not in the app folder. I didn't write them and I don't want them cluttering my app (bower_components, scripts, lib).

Note: Find more details and reasoning behind the structure at this 
<a href="http://www.johnpapa.net/angular-app-structuring-guidelines/">original post</a> on application structure.


### Layout

Place components that define the overall layout of the application in a folder named layout. These may include a shell view and controller may act as the container for the app, navigation, menus, content areas, and other regions.

Why?: Organizes all layout in a single place re-used throughout the application.



### Folders-by-Feature Structure

Create folders named for the feature they represent. When a folder grows to contain more than 7 files, start to consider creating a folder for them. Your threshold may be different, so adjust as needed.

Why?: A developer can locate the code, identify what each file represents at a glance, the structure is flat as can be, and there is no repetitive nor redundant names.

Why?: The LIFT guidelines are all covered.

Why?: Helps reduce the app from becoming cluttered through organizing the content and keeping them aligned with the LIFT guidelines.

Why?: When there are a lot of files (10+) locating them is easier with a consistent folder structures and more difficult in flat structures.

```{
/**
 * recommended
 */

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
        session-detail.controller.js
}```













