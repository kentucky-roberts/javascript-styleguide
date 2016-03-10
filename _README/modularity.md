# Modularity

#### Many Small, Self Contained Modules

Create small modules that encapsulate one responsibility.

Why?: Modular applications make it easy to plug and go as they allow the development teams to build vertical slices of the applications and roll out incrementally. This means we can plug in new features as we develop them.



## Create an App Module

[Style Y161]

Create an application root module whose role is to pull together all of the modules and features of your application. Name this for your application.

Why?: Angular encourages modularity and separation patterns. Creating an application root module whose role is to tie your other modules together provides a very straightforward way to add or remove modules from your application.