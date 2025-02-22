---
id: 72c7218e-1a9f-49a6-904d-ed8588e57869
blueprint: sections
title: 'Extending'
intro: While Statamic contains countless features, you are free to add more, or modify existing ones.
template: extending.index
section: extending_docs
---
## To addon, or not to addon?

Since Statamic is a Laravel package, you are in control over your application code.

**If you want to reuse, distribute, or sell your features; you should make an addon.** Otherwise, you can just add things to your Laravel application.

## How to extend Statamic

Many features can simply be placed in the right spot and they'll be wired up automatically.

For example, placing a [Tag](/extending/tags) class inside `app/Tags` will make it available to your templates without any extra wiring.
Or if you're building an addon, putting it in `src/Tags` will do the same.

Others could require some wiring, which would typically go in a service provider.

## How **not** to extend Statamic {#how-not-to-extend-statamic}

It should go without saying — but we'll say it anyway just in case...

Don't ever, for any reason, ever, no matter what, no matter where, or who, or who you are with, or where you are going or... or where you've been... ever, for any reason, whatsoever, edit the files inside `/vendor/statamic`. Or any other Composer package. Anything you do will get blown away and you'll lose those changes forever and ever amen.

You should instead build addons, extensions, and submit pull requests to [core](https://github.com/statamic/cms) (after checking with the team first if we'll accept them). Thanks! 
