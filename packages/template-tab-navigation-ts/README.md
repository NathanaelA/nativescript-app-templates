# NativeScript Core with TypeScript Tab Navigation Template
App templates help you jump start your native cross-platform apps with built-in UI elements and best practices. Save time writing boilerplate code over and over again when you create new apps.

App template featuring a TabView component for navigation.

<img src="/packages/template-tab-navigation-ts/tools/assets/phone-tab-ios.png" height="400" /> <img src="/packages/template-tab-navigation-ts/tools/assets/phone-tab-android.png" height="400" />

## Key Features
- Tab navigation
- Five blank pages hooked to the tab navigation
- Customizable theme
- UX and development best practices
- Easy to understand code through extensive code comments

## Quick Start
Execute the following command to create an app from this template:

```
tns create my-tab-ts --template tns-template-tab-navigation-ts
```

> Note: This command will create a new NativeScript app that uses the latest version of this template published to [npm](https://www.npmjs.com/package/tns-template-tab-navigation-ts).

If you want to create a new app that uses the source of the template from the `master` branch, you can execute the following:

```
# clone nativescript-app-templates monorepo locally
git clone git@github.com:NativeScript/nativescript-app-templates.git

# create app template from local source (all templates are in the 'packages' subfolder of the monorepo)
tns create my-tab-ts --template nativescript-app-templates/packages/template-tab-navigation-ts
```

**NB:** Please, have in mind that the master branch may refer to dependencies that are not on NPM yet!

## Walkthrough

### Architecture
The application root component is located at:
- `app-root.xml` - sets up the tab navigation page layout and references the navigatable pages contents.

The template has the following pages used for the tab views:
- `/home/home-items-page.ts` - the master home page. Displays a list of items and navigates to the item details page on item tap.
- `/home/home-item-detail/home-item-detail-page.ts` - the item details page. Displays the details of the tapped item.
- `/browse/browse-page.ts` - blank page
- `/search/search-page.ts` - blank page

### Styling
This template is set up to use SASS for styling. All classes used are based on the {N} core theme – consult the [documentation](https://docs.nativescript.org/angular/ui/theme.html#theme) to understand how to customize it. Check it out to see what classes you can use on which component.

It has 4 global style files that are located at the root of the app folder:
- `_app-variables.scss` - holds the global SASS variables that are imported on each component's styles.
- `app.scss` - the global common style sheet. These style rules are applied to both Android and iOS.
- `platform.android.scss` - the global Android style sheet. These style rules are applied to Android only.
- `platform.ios.scss` - the global iOS style sheet. These style rules are applied to iOS only.

Each component has 3 style files located in the its folder:
- `_page-name.scss` - the component common style sheet. These style rules are applied to both Android and iOS.
- `page-name.android.scss` - the component Android style sheet. These style rules are applied to Android only.
- `page-name.ios.scss` - the component iOS style sheet. These style rules are applied to iOS only.

## Get Help
The NativeScript framework has a vibrant community that can help when you run into problems.

Try [joining the NativeScript community Slack](http://developer.telerik.com/wp-login.php?action=slack-invitation). The Slack channel is a great place to get help troubleshooting problems, as well as connect with other NativeScript developers.

If you have found an issue with this template, please report the problem in the [NativeScript repository](https://github.com/NativeScript/NativeScript/issues).

## Contributing

We love PRs, and accept them gladly. Feel free to propose changes and new ideas. We will review and discuss, so that they can be accepted and better integrated.
