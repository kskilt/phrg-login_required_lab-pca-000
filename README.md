# Login Required Lab

## Objectives

We're going to make a Rails app that requires you to be logged in to see one of its pages.

## Introduction

Our app has three pages:
  1. A login page, where the user enters their username. No passwords; we'll just trust them. After they're logged in, users are taken to...
  2. A user homepage, which says, "Hi, #{username}", and has a link to the secret page, which is...
  3. A page with a secret on it, which users must be logged in to see.

## Instructions

1. Build out the `SessionsController`.

2. Write a `current_user` method.

3. Write a `SecretsController` using a `before_action` to prevent any route from being accessed without logging in.

Use the specs as your guide, but we'd like the following behavior. We should be able to:
  * Visit the root of the app and be redirected to a login page.
  * If a user fails to enter their name on the login page, they should be redirected there until they successfully do so.
  * Once logged in, a user should see the welcome page. This page should greet the user and link them to the secret page.
  * The content and URL of the secret page are up to you. However, if we visit that URL without logging in, we should be redirected to the login page. Under no circumstances should we allow people who are not logged in to see the secrets.

Happy coding!

## Does this need an update?
 Please open a [GitHub issue](https://github.com/learn-co-curriculum/phrg-login_required_lab/issues) or [pull-request](hhttps://github.com/learn-co-curriculum/phrg-login_required_lab/pulls). Provide a detailed description that explains the issue you have found or the change you are proposing. Then "@" mention your instructor on the issue or pull-request, and send them a link via Connect.

<p data-visibility='hidden'>PHRG Login Required Lab</p>
