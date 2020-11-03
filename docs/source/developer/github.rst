Git and Github
==============

..  toctree::
    :maxdepth: 3

    /developer/github

--------------

Getting Started with Github
---------------------------

Instead of reinventing the wheel, there are countless trainings online.
Here are few good ones we have found: \*
Lynda.com: https://www.lynda.com/Git-training-tutorials/1383-0.html \*
TBD

Github Notifications
--------------------

Github email notifications can become very difficult to parse through without proper 
email management and setup. The following section helps you pull high priority emails 
out to ensure you do not miss out on various activities that require your more immediate 
attention.

Setup Notifications
~~~~~~~~~~~~~~~~~~~

To ensure you are up-to-date with all things happening in repositories,
check your `notification
settings <https://github.com/settings/notifications>`__ send you emails
/ mobile notifications when needed. For PDS development, at minimum,
please check the following: 

* **Participating:**
   ✅ Email
   ✅ Web and Mobile

* **Watching:**
   ✅ Email
   ✅ Web and Mobile

Managing Repository Notifications
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

You can manage the notifications you receive for specific repositories from here: 
https://github.com/watching . From this page, you can determine what types of notifications 
you would like to receive from repositories you are watching.

For more information on managing notifications, see the `Github documentation <https://help.github.jp/enterprise/2.11/user/articles/watching-and-unwatching-repositories/>`_

@mentions Email Filter
~~~~~~~~~~~~~~~~~~~~~~

Think of a Github @mention as a direct message, versus other issue and
commit notifications being group messages. It is highly recommended you
setup an email filter to pull out these @mentions (aka direct messages)
so you are able to respond in a timely manner.

Here is an example email filter from Microsoft Exchange:

::

   When a new message arrives that meets all these conditions:
     Body     Contains    @my_username
     Sent To  Contains    mention@noreply.github.com
     From     Contains    github.com

   Do the following:
     Move to Folder      Github-@mentions (you will need to create this folder)

   [checked] Do not apply other rules to message that meet the same conditions

   [checked] Enabled


Pull Requests Review Requested Email Filter
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In order to prioritize pull request reviews above other Github email notifications, 
this email filter will help you pull out emails where your review is requested.

Note: This applies to both personal reviews and reviews requested of a team you belong to.

Here is an example email filter from Microsoft Exchange:

::

   When a new message arrives that meets all these conditions:
     Body     Contains    your review
     Sent To  Contains    review_requested@noreply.github.com
     From     Is          notifications@github.com

   Do the following:
     Move to Folder      Github-@reviews (you will need to create this folder)

   [checked] Do not apply other rules to message that meet the same conditions

   [checked] Enabled


Github Notifications Email Filter
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This email filter is intended to be a catchall for remaining github notifications for a particular organization. This can be adapted to handle individual repositories as you see fit.

NOTE: Make sure this is the last email filter in your list, otherwise the filters created above will be ignored.

Here is an example email filter for the `NASA-PDS Github Org <https://github.com/NASA-PDS/>`_ through Microsoft Exchange:

::

   When a new message arrives that meets all these conditions:
     Subject  Contains    NASA-PDS/
     From     Contains    "noreply@github.com" or "notifications@github.com"

   Do the following:
     Move to Folder      PDS-Github (you will need to create this folder)

   [checked] Do not apply other rules to message that meet the same conditions

   [checked] Enabled


Here is an example email filter for the `PDS-Data-Dictionaries Github Org <https://github.com/pds-data-dictionaries/>`_ through Microsoft Exchange:

::

   When a new message arrives that meets all these conditions:
     Subject  Contains    pds-data-dictionaries/
     From     Contains    "noreply@github.com" or "notifications@github.com"

   Do the following:
     Move to Folder      pds-ldd-github (you will need to create this folder)

   [checked] Do not apply other rules to message that meet the same conditions

   [checked] Enabled


Commit Message Best Practices
-----------------------------

For commit message best practices, the PDS tries to follow these `Github
Commit Messages
Guidelines <https://gist.github.com/robertpainsi/b632364184e70900af4ab688decf6f53>`__
where possible.

Once you have read through the guidelines, here are some highlights to
touch on and some additional notes:

A properly formed git commit subject line should always be able to
complete the following sentence

::

   If applied, this commit will <your subject line here>

-  **Rules for a great commit message style**

   -  Separate subject from body with a blank line
   -  Do not end the subject line with a period
   -  Capitalize the subject line and each paragraph
   -  Use the imperative mood in the subject line
   -  Wrap lines at 72 characters
   -  Use the body to explain what and why you have done something. In
      most cases, you can leave out details about how a change has been
      made.

-  **References in commit messages**

   -  If the commit refers to an issue, add this information to the
      commit message header or body.
   -  See `how to autolink references and
      urls <https://help.github.com/en/github/writing-on-github/autolinked-references-and-urls>`__
      for more information on linking to other issues, repos, commits,
      etc.
   -  Do this for ticket references, people, etc.
   -  Be sure use the correct referencing method when going across
      repositories.

::

   Short (72 chars or less) summary

   More detailed explanatory text. Wrap it to 72 characters. The blank
   line separating the summary from the body is critical (unless you omit
   the body entirely).

   Write your commit message in the imperative: "Fix bug" and not "Fixed
   bug" or "Fixes bug." This convention matches up with commit messages
   generated by commands like git merge and git revert.

   Further paragraphs come after blank lines.

   - Bullet points are okay, too.
   - Typically a hyphen or asterisk is used for the bullet, followed by a
     single space. Use a hanging indent.

For example:

::

   $ git add my_file.txt

   # Try to avoid using `git commit -m` unless it is a very trivial update/change
   $ git commit

   # Vim or Emacs window will open. To change editor that opens, see https://help.github.com/en/github/using-git/associating-text-editors-with-git .
   Created new my_file with text in it

   This new file includes:
   * Part 1
   * Part 2
   * Part 3

Issue Tracking
--------------

See more information at `PDS Issue Tracking
Guide <pds_issue_tracking_guide.md>`__

Advanced Help
-------------

Help With Rebasing
~~~~~~~~~~~~~~~~~~

Rebasing can get messy and be painful. We highly recommend reading this
article on `The Golden Rule of
Rebasing <https://www.atlassian.com/git/tutorials/merging-vs-rebasing#the-golden-rule-of-rebasing>`__.

References
----------

-  https://help.github.com/en/github/writing-on-github/autolinked-references-and-urls
