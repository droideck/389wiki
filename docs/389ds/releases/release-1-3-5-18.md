---
title: "Releases/1.3.5.18"
---

389 Directory Server 1.3.5.18
-----------------------------

The 389 Directory Server team is proud to announce 389-ds-base version 1.3.5.18.

Fedora packages are available from the Fedora 24, and 25.

The new packages and versions are:

-   389-ds-base-1.3.5.18-1

Source tarballs are available for download at [Download 389-ds-base Source]({{ site.binaries_url }}/binaries/389-ds-base-1.3.5.18.tar.bz2) and [Download nunc-stans Source]({{ site.binaries_url }}/binaries/nunc-stans-0.1.8.tar.bz2).

### Highlights in 1.3.5.18

-   Bug fixes

### Installation and Upgrade

See [Download](../download.html) for information about setting up your yum repositories.

To install, use **yum install 389-ds** yum install 389-ds After install completes, run **setup-ds-admin.pl** if you have an Admin Server installed (389-admin), otherwise just run **setup-ds.pl** to set up your directory server.

To upgrade, use **yum upgrade** yum upgrade After upgrade completes, run **setup-ds-admin.pl -u** if you have an Admin Server installed (389-admin), otherwise just run **setup-ds.pl -u** to update your directory server/admin server/console information.

See [Install\_Guide](../legacy/install-guide.html) for more information about the initial installation, setup, and upgrade

See [Source](../development/source.html) for information about source tarballs and SCM (git) access.

### Feedback

We are very interested in your feedback!

Please provide feedback and comments to the 389-users mailing list: <https://lists.fedoraproject.org/admin/lists/389-users.lists.fedoraproject.org> as well as: 

F24 <https://bodhi.fedoraproject.org/updates/FEDORA-2017-f0ace457f7>
F25 <https://bodhi.fedoraproject.org/updates/FEDORA-2017-a4824a5fb4>


If you find a bug, or would like to see a new feature, file it in our Trac instance: <https://pagure.io/389-ds-base/new_issue>

- Bump version to 1.3.5.18
- Ticket 49273 - Fix logging from previous patch
- Ticket 49273 - bak2db doesn't operate with dbversion
- Ticket 49273 - crash when DBVERSION is corrupt.
- Ticket 49241 - add symblic link location to db2bak.pl output
- Ticket 49157 - fix error in ds-logpipe.py
- Ticket 49246 - ns-slapd crashes in role cache creation
- Ticket 48989 - Re-implement lock counter
- Ticket 48989 - missing return in counter
- Ticket 48989 - Improve counter overflow fix
- Ticket 49157 - ds-logpipe.py crashes for non-existing users
- Ticket 49241 - Update man page and usage for db2bak.pl
- Ticket 49209 - Hang due to omitted replica lock release

