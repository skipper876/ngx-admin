# Ngx-Admin from akveo with Firebase (using AngularFire2)

## Firebase auth with the template of akveo/nebular/auth
The akveo auth provider is not needed anymore.

I added a new auth provider that is connected to your firebase app.

You will have the same look than akveo/ngx-admin.

You need to go to the app.module to add your own firebase config.

## Login and register page
Email and password authentification is easy !

## Login and register using Connect with Google, Facebook... mechanics also based on firebase
On login and register you have "connect with" buttons are linked to your firebase auth mechanics.

To edit them also go to @core/core.module.ts and add the specific function in register and login.

Example : 

const socialLinks = [
  {
    name: "facebook",
    icon: 'socicon-facebook',
  },... ]

Register mecanics for google and facebook is not completly finished. Contributions are welcome.

They work but does not triggers everything yet.

Login "connect with" is fine.

## Reset Password

"Request password" page with ask firebase to send an email.

The email should link to the "reset password" page.

Then the "code" is in the link (parameter oobCode) is extracted from the url to secure the password change.

## Other note

I added a additional field on the register to show you how to store additional info on firestore.

-----------------------------------------------------------

-----------------------------------------------------------

# Original read me by Akveo

[![Build Status](https://travis-ci.org/akveo/ngx-admin.svg?branch=master)](https://travis-ci.org/akveo/ngx-admin)
[![Join the chat at https://gitter.im/ng2-admin/Lobby](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/ng2-admin/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Dependency Status](https://david-dm.org/akveo/ngx-admin/status.svg)](https://david-dm.org/akveo/ng2-admin)
# Admin template based on Angular 5+, Bootstrap 4 and <a href="https://github.com/akveo/nebular">Nebular</a>
<a target="_blank" href="http://akveo.com/ngx-admin/#/pages/dashboard?utm_source=github&utm_medium=ngx_admin_readme&utm_campaign=demo"><img src="https://i.imgur.com/XoJtfvK.gif"/></a>

### Two themes available:

| Cosmic Theme | Business Theme |
|:------------:|:--------------:|
|<a target="_blank" href="http://akveo.com/ngx-admin/#/pages/dashboard?theme=cosmic&utm_source=github&utm_medium=ngx_admin_readme&utm_campaign=themes"><img src="https://i.imgur.com/FgRZcqL.png"/></a>|<a target="_blank" href="http://akveo.com/ngx-admin/#/pages/dashboard?theme=default&utm_source=github&utm_medium=ngx_admin_readme&utm_campaign=themes"><img src="https://i.imgur.com/fozHlRJ.png"/></a>|

### What's included:

- Angular 5+ & Typescript
- Bootstrap 4+ & SCSS
- Responsive layout
- High resolution
- Flexibly configurable themes with **hot-reload** (2 themes included)
- Authentication module with multiple providers
- Lots of awesome features:
  - Buttons
  - Modals
  - Popovers
  - Icons
  - Typography
  - Animated searches
  - Forms
  - Tabs
  - Notifications
  - Tables
  - Maps
  - Charts
  - Editors
  
And many more!

### Demo

<a target="_blank" href="http://akveo.com/ngx-admin/">Live Demo</a>

## Documentation
This template is using [Nebular](https://github.com/akveo/nebular) modules set, [here you can find documentation and other useful articles](https://akveo.github.io/nebular/#/docs/installation/based-on-starter-kit-ngxadmin).

### ng2-admin
We will continue supporting [ng2-admin](https://github.com/akveo/ngx-admin/tree/ng2-admin) version, but if you are starting from scratch we recommend using `ngx-admin`. Unfortunately, there is no way to automatically update from ng2-admin to ngx-admin, but some parts (Nebular components) could be manually included.

### Empty starter kit
Don't need all the pages and modules and just looking for an empty starter kit for your next project? Check out our [starter-kit branch](https://github.com/akveo/ngx-admin/tree/starter-kit).

### Angular 1.x version
Here you can find Angular 1.x based version: [Blur Admin](http://akveo.github.io/blur-admin/)

## BrowserStack
This project runs its tests on multiple desktop and mobile browsers using [BrowserStack](http://www.browserstack.com).

<img src="https://cloud.githubusercontent.com/assets/131406/22254249/534d889e-e254-11e6-8427-a759fb23b7bd.png" height="40" />

### How can I support developers?
- Star our GitHub repo :star:
- Create pull requests, submit bugs, suggest new features or documentation updates :wrench:
- Follow us on [Twitter](https://twitter.com/akveo_inc) :feet:
- Like our page on [Facebook](https://www.facebook.com/akveo/) :thumbsup:

### Looking for engineering services? 
Visit [our homepage](http://akveo.com/) or simply leave us a message to [contact@akveo.com](mailto:contact@akveo.com). We will be happy to work with you!

### From Akveo
Made with :heart: by [Akveo team](http://akveo.com/). Follow us on [Twitter](https://twitter.com/akveo_inc) to get the latest news first!
We're always happy to receive your feedback!
