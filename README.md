# drupal-ops
Mega Repo for Drupal Ops Tools

## What?

Drupal Ops is a set of Drupal modules for managing sites, servvers, and tasks.

This repo will contain all components. Git Split is used to push out individual modules.

## How?

- `composer require drupal/site`
- `composer require drupal/server`
- `composer require drupal/task`

Each module works independently to provide intelligence to your Drupal sites.

## Development

This is just a Drupal site, using a composer stack.

Clone it into your favorite Drupal site tool.

## Components

1. **Drupal Tasks**: `drupal/task`
  - Provides an Entity representing a command and it's results.
  - Stores a command, arguments, logs and process metadata.
  - Create a task then run it later from a command line.
  - Use provided Task Types or create your own with Field UI.
  - Capture commands run from the CLI to save history regardless of where the command was initiated.
2. **Drupal Sites**: `drupal/site`
  - Provides an entity representing a Drupal website.
  - Stores properties such as domain, domain aliases, Site type (dev, etc), Site UUID, Git repository, Git Reference, Install Profile.
  - When added to a Drupal site, provides a Site Entity automatically generated from the current site.
  - Provides ability to track additional properties about a site, such as last backup, database stats, 

## History

Many ages ago, the god of the seas, Aegir, gained the ability to create Drupal, using Drupal.

That system contained Drupal modules called `hosting_site`, `hosting_server` and `hosting_task`.

Some time passed, and Aegir begat OpenDevShop: a more developer friendly version of Aegir.

Drupal Ops tooling is being created using lessons learned in those projects.

## Credits

Drupal-Ops was created by Jon Pugh, ThinkDrop Inc.

