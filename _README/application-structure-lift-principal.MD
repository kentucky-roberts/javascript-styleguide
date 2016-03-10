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