---
id: 61c8db2d-f7bf-4829-bafd-f8a4db5a9a57
blueprint: page
title: 'Install Statamic Locally Using Laravel Herd'
nav_title: Herd
intro: 'Using Laravel Herd to run Statamic locally is the **easiest and fastest way** to get started with the best CMS. It is also very **beginner-friendly**.'
parent: ab08f409-8bbe-4ede-b421-d05777d292f7
---
## Overview

Laravel Herd offers a straightforward approach to setting up your machine with all the necessary dependencies for PHP development, like a web server and Composer. It's easier than using Homebrew, less error-prone, and blazingly fast. It's our preferred and recommended way to get started with Statamic and Laravel development in general on a Mac.

## Prerequisites

To install Herd and run Statamic locally you will need the following:

- A Macintosh running macOS 12.0+
- That's it.

## Install Laravel Herd

Installing Herd is super easy and the same process as with any other application on the Mac. Just [download the latest version](https://herd.laravel.com/download), open the `.dmg` file, and drop the app into your `Applications` folder.

<figure>
    <img src="/img/herd-dmg-finder.jpg" alt="">
    <figcaption>Drag'n'Drop It Like It's Hot </figcaption>
</figure>

After you open it for the first time, you will get prompted to type in your password so all the necessary files can be put in the right places.

<figure>
    <img src="/img/herd-password-prompt.jpg" alt="">
</figure>

If you previously used Laravel Valet you can migrate to Herd and all settings, like linked projects and installed PHP versions, will be synced. Didn't use Valet before? Then you won't see this screen.

<figure>
    <img src="/img/herd-valet-detected.jpg" alt="">
</figure>

Next, you get presented with a screen saying that you can now use Herd, Composer, and more. The default location to place your projects is `~/Herd`. You can also choose to automatically launch Herd on startup which we would recommend.

<figure>
    <img src="/img/herd-installation-success.jpg" alt="">
</figure>

After that's done, Herd has been successfully installed and you now have a local PHP dev environment on your machine.

<figure>
    <img src="/img/herd-menu-bar-item.jpg" alt="">
    <figcaption>Harold congratulates you from Hungary 🇭🇺</figcaption>
</figure>

If you want to install additional PHP versions or make your local sites available through [Expose](http://expose.dev/) via secure tunnels, open the Herd settings to get access to a range of different options.

<figure>
    <img src="/img/herd-settings-php-versions.jpg" alt="">
</figure>

## Install Statamic CLI

Next up on your journey to greatness is installing the Statamic CLI. To do this, run the following command in your terminal:

``` shell
composer global require statamic/cli
```

Upon installation, you can now use `statamic new` to spin up fresh Statamic sites with a CLI setup wizard 🧙‍♂️ to guide you through a range of settings and options.

Our CLI is essentially a super fancy wrapper around the `composer create-project` command. You can choose to not install it. Though it offers a wide range of really neat features and we recommend it.

## Create a new site

Let's take the last big step towards you enjoying all of Statamic radness™.

In your terminal, run `statamic new your-project-name` and follow the steps and prompts to create a new site.

<figure>
    <img src="/img/herd-statamic-cli.jpg" alt="">
    <figcaption>Hot pink and sweet lookin' 💅</figcaption>
</figure>

For a more in-depth guide on using the CLI and all of its options, have a look at [its docs](/cli).

## Access the site

Sweet, if you did all the previous steps you should now be able to open your site at  `http://your-project-name.test`.

<figure>
    <img src="/img/herd-fresh-statamic-site.jpg" alt="">
</figure>

The Control Panel, Statamic's admin area, can be accessed at `/cp`.

## What's Next

Well done, you have turned your computer into a local PHP development environment, installed the Statamic CLI, and set up your first Statamic site! 🎉

Get creative, explore everything, and build something rad.

Want to learn more about Statamic? Watch [our series on Laracasts](https://laracasts.com/series/learn-statamic-with-jack) or just continue to browse through the docs.

For additional information on Laravel Herd, have a look at its [documentation](https://herd.laravel.com/docs).

:::tip
Use all of Statamic's Pro features while in development (like unlimited users, permissions, GraphQL, REST API, and more), by setting `'pro' => true` in `config/statamic/editions.php`.
:::
