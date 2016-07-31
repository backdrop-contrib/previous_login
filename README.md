Previous login
==============

Add a detective security control to Backdrop by displaying the previous login timestamp after a successful login.

By reporting the previous login, users have the opportunity to notice and report suspicious logins. Users who notice previous login timestamps which do not match their previous interactions should report the event to their administrator for investigation.

This module may help detect when a user had their password stolen, a session hijacked, or a database compromise. By detecting unauthorized logins, administrators are alerted to save system logs to review for where unauthorized activity may have originated from and what actions were performed.

Configuration
-------------

The Previous login module doesn't have configuration of its own, but its usefulness depends on the Backdrop core regional configuration.

Since the default settings for Backdrop will use UTC for all site timestamps, users in the EST/EDT could see their previous login timestamp offset by 4 hours if the administrator does not allow regional timezone settings.

Review your configuration at:

Administration » Configuration » Regional and language » Regional settings

The recommended configuration is to allow users to configure their own timezones for each account: "Users may set their own time zone."

Login Security
--------------

This functionality was bolted on to the Login Security module in Drupal. As the Login Security module grew, it became bloated. This module brings specific functionality without bloat or configuration overhead of unrelated features.

Current Maintainer
------------------

- David Norman (https://github.com/deekayen)

Credits
-----------

- Originally written as part of the Login Security module for Drupal
  (https://www.drupal.org/project/login_security)
- Ported to Backdrop by David Norman (https://github.com/deekayen)

License
-------

This project is GPL v2 software. See the LICENSE.txt file in this directory for
complete text.
