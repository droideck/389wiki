---
title: "Releases/1.3.1.12"
---
389 Directory Server 1.3.1.12
-----------------------------

The 389 Directory Server team is proud to announce 389-ds-base version 1.3.1.12.

Fedora packages are available from the Fedora 19 Testing repositories.

The new packages and versions are:

-   389-ds-base-1.3.1.12-1

A source tarball is available for download at [Download Source]({{ site.binaries_url }}/binaries/389-ds-base-1.3.1.12.tar.bz2)

### Highlights in 1.3.1.12

-   server should restart cleanly after reboot - tmpfiles.d issues with /run have been resolved
    -   This time the issue has really been resolved
-   logconv.pl improvements
-   bug fixes

### Installation and Upgrade

See [Download](../download.html) for information about setting up your yum repositories.

To install, use **yum install 389-ds** yum install 389-ds After install completes, run **setup-ds-admin.pl** to set up your directory server. setup-ds-admin.pl

To upgrade, use **yum upgrade** yum upgrade After upgrade completes, run **setup-ds-admin.pl -u** to update your directory server/admin server/console information. setup-ds-admin.pl -u

See [Install\_Guide](../legacy/install-guide.html) for more information about the initial installation, setup, and upgrade

See [Source](../development/source.html) for information about source tarballs and SCM (git) access.

### Feedback

We are very interested in your feedback!

Please provide feedback and comments to the 389-users mailing list: <https://lists.fedoraproject.org/admin/lists/389-users.lists.fedoraproject.org>

If you find a bug, or would like to see a new feature, file it in our Trac instance: <https://fedorahosted.org/389>

### Detailed Changelog since 1.3.1.11

-   Ticket 53 - Need to update supported locales
-   Ticket 54 - locale "nl" not supported by collation plugin
-   Ticket 47354 - Indexed search are logged with 'notes=U' in the access logs
-   Ticket 47387 - improve logconv.pl performance with large access logs
-   Ticket 47501 - logconv.pl uses /var/tmp for BDB temp files
-   Ticket 47513 - tmpfiles.d references /var/lock when they should reference /run/loc
-   Ticket 47517 - memory leak in range searches and other various leaks
-   Ticket 47520 - Fix various issues with logconv.pl
-   Ticket 47522 - Password adminstrators should be able to voilate password policy
-   Ticket 47543 - Mozldap - fix compiler warnings
-   Ticket 47551 - logconv: -V does not produce unindexed search report
-   Ticket 47533 - logconv: some stats do not work across server restarts
-   Coverity fixes - 12023, 12024, and 12025

