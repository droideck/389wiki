---
title: "Download"
---

# Download 389 Directory Server
-------------------------------

Below you will find links to download the binary packages and source files. Please see the [FAQ section on Open Source](FAQ/faq.html#open-source) for more information.

<div style="text-align: left;">
<span style="display:inline-block;padding:1px;border:1px solid #000;font-size:80%;">
EXPORT CONTROL. As required by U.S. law, you (Licensee) represents and warrants that it: (a) understands that the Software is subject to export controls under the U.S. Commerce Department's Export Administration Regulations ("EAR"); (b) is not located in a prohibited destination country under the EAR or U.S. sanctions regulations (currently Cuba, Iran, Iraq, North Korea, Sudan and Syria); (c) will not export, re-export, or transfer the Software to any prohibited destination, entity, or individual without the necessary export license(s) or authorizations(s) from the U.S. Government; (d) will not use or transfer the Software for use in any sensitive nuclear, chemical or biological weapons, or missile technology end-uses unless authorized by the U.S. Government by regulation or specific license; (e) understands and agrees that if it is in the United States and exports or transfers the Software to eligible end users, it will, as required by EAR Section 740.17(e), submit semi-annual reports to the Commerce Department's Bureau of Industry & Security (BIS), which include the name and address (including country) of each transferee; and (f) understands that countries other than the United States may restrict the import, use, or export of encryption products and that it shall be solely responsible for compliance with any such import, use, or export restrictions.
</span>
</div>
<br>

{% include toc.md %}

## Binary Packages
------------------

### RHEL/CentOS/EPEL (RHEL 6, RHEL 7, CentOS 6, CentOS 7)

**NOTE**: Use the 389-ds-base package from your base distribution.  389-ds-base is part of RHEL and CentOS now.  The copr repositories are discontinued.

**NOTE**: The EL7 admin server and console bits will not be available until after RHEL 7.1 has been released.  These bits will then be available from EPEL7.

For the admin server and console bits, you must first install EPEL from <https://fedoraproject.org/wiki/EPEL>. There is no direct link to the RPM, you must first find a mirror. Go here to find the RPM:

[EPEL 6](http://download.fedoraproject.org/pub/epel/6/x86_64/repoview/epel-release.html)
[EPEL 7](http://download.fedoraproject.org/pub/epel/7/x86_64/repoview/epel-release.html)

That will direct you to a mirror where you can download the epel-release X (6 or 7) RPM:

    yum install http://site/path/to/epel-release-X-N.noarch.rpm

Then you can install 389-ds-base and get all of the core directory server, admin server, and console components as per the directions below.

### 389 Directory Server 1.1 and later

-   yum is used to install on platforms that use yum for package installation and management.
-   Enterprise Linux packages are available from EPEL
    -   How to use - <https://fedoraproject.org/wiki/EPEL/FAQ#howtouse>
    -   More info on EPEL - <https://fedoraproject.org/wiki/EPEL>

New Install:

    yum install 389-ds-base
    setup-ds-admin.pl

Upgrade an existing system:

    yum [--enablerepo=updates-testing|--enablerepo=epel-testing] upgrade [389-ds-base ...other packages...]
    setup-ds-admin.pl -u

If you specify package names on the command line, only those packages will be updated - useful for testing, if you just want to test certain packages without upgrading every package on your system to the testing version. You can use *yum downgrade pkgname ... pkgname* to downgrade the package from the testing version to the stable version.

-   Testing - installing packages from the testing repos
    -   On Fedora - yum install 389-ds-base --enablerepo=updates-testing
    -   On EPEL - yum install 389-ds-base --enablerepo=epel-testing
    -   On Fedora - yum upgrade <testing packages> --enablerepo=updates-testing
    -   On EPEL - yum upgrade <testing packages> --enablerepo=epel-testing
    -   See the [Release Notes](releases/release-notes.html) for the current list of testing packages
-   Upgrade - **yum upgrade**
    -   The 389 packages are designed to obsolete and replace the fedora-ds packages - you must use yum **upgrade** *not update* in order for yum and rpm to process the obsolete directives
    -   You **must** run **setup-ds-admin.pl -u** after the upgrade to refresh your admin server and console configuration
-   New Install - **yum install 389-ds-base**
    -   Run **setup-ds-admin.pl** to set up your directory server

Upgrading and installing will install many dependencies too, including Java if your platform supports it. If not, see [Install Guide](legacy/install-guide.html) for more information about Java.

See [Install Guide](legacy/install-guide.html) for more information.

### Windows Password Synchronization

NOTE: If you are upgrading from version **1.1.0**, the upgrade will create a new 389 Password Sync folder and copy your files from the old Fedora Password Sync folder. It will not remove the old Fedora Password Sync folder. You can do that manually once you have verified that the new 389 version is working correctly.

NOTE: If you are upgrading from a version older than **1.1.0**, install the new version first, then remove the old version from the Add/Remove Programs list in the Control Panel. The new version is **1.1.7**.

This is an Active Directory "plug-in" that intercepts password changes made to AD Domain Controllers and sends the clear text password over an encrypted connection (SSL/TLS) to 389 DS to keep the passwords in sync. It works in conjunction with the Windows Sync feature of 389. You must install this on every Domain Controller.

Tested with Windows 2008 and 2012 Server 32-bit and 64-bit.

|Platform|File|SHA1SUM|SSLv3|>=TLSv1.1|
|--------|----|-------|-----|---------|
|Windows 2003/2008 32-bit|[389-PassSync-1.1.5-i386.msi]({{ site.binaries_url }}/binaries/389-PassSync-1.1.5-i386.msi)|4b79578e3d4bf9cdaada70e5c1212290a4e5ce3c|yes|no [*]|
|Windows 2003/2008 64-bit|[389-PassSync-1.1.5-x86\_64.msi]({{ site.binaries_url }}/binaries/389-PassSync-1.1.5-x86_64.msi)|ddac9705d305b14fa217af2f264d3529d3f3edb8|yes|no [*]|
|Windows 2003/2008/2012 32-bit|[389-PassSync-1.1.7-i386.msi]({{ site.binaries_url }}/binaries/389-PassSync-1.1.7-i386.msi)|780e403335a74ea58dc097fb60fd481c8457e105|no [**]|yes|
|Windows 2003/2008/2012 64-bit|[389-PassSync-1.1.7-x86\_64.msi]({{ site.binaries_url }}/binaries/389-PassSync-1.1.7-x86_64.msi)|0d598943ecdd17eeca2d66174de18d9885951699|no [**]|yes|

[*] 389-PassSync-1.1.5 has no support TLSv1.1 and newer.

[**] 389-PassSync-1.1.7 disables SSLv3 by default.

### Windows Console

NOTE: Windows Console now (as of September 11, 2015) requires Java 7 to work.

NOTE: You must use 64-bit Java with the 64-bit version.

Tested with Java 7 on Windows 2008/2012 Server.

|Platform|File|SHA1SUM|
|--------|----|-------|
|Windows 2008/2012 32-bit|[389-Console-1.1.15-i386.msi]({{ site.binaries_url }}/binaries/389-Console-1.1.15-i386.msi)|772e4691daea66dcdef97cb220d9ae77ab9fbe78|
|Windows 2008/2012 64-bit|[389-Console-1.1.15-x86\_64.msi]({{ site.binaries_url }}/binaries/389-Console-1.1.15-x86_64.msi)|35ec5bad0d309c334ba8c5e8ac0ab183f004d7fd|

NOTE: You must have Java in your PATH in order for this to work. Or you can just edit the batch file to tell it where to find Java.

<br>

## Legacy Releases
------------------

These releases are very old, and provided for historical purposes only.

### Windows Synchronization

The following is only required for NT4 sync. It is not required for Active Directory sync.

-   [NTDS]({{ site.binaries_url }}/binaries/ntds.msi) md5sum 74e0ada5ff519ade5295ae0bf75ddb84

### Fedora Directory Server 1.x 

These rpm packages are no longer available for download, but the source code for each version is, and they can be located [here]({{ site.binaries_url }}/binaries/)

### Fedora Directory Server 7.1

The FDS 7.1 package includes the core DS, the Admin Server, the Management Console, web applications, and other support code for those apps, including online help. Since the Admin Server and related files in this legacy package are not available as open source, please refer to the [Licensing](FAQ/licensing.html) for these Binary packages. 

-   [FDS 7.1 Source Code]({{ site.binaries_url }}/binaries/fedora-ds-7.1.tar.gz)
-   [FDS 7.1 SRPM]({{ site.binaries_url }}/binaries/fedora-ds-7.1-2.src.rpm)


## Source Code Packages
-----------------------

Check out our [Build](development/building.html) page to find out how to build from source. The source packages are available [here](development/source.html).

## Scripts
----------

Checkout our scripts page [here](scripts.html)

## Schema
----------

Checkout our schema page [here](schema.html)

## Artwork and logos
--------------------

We maintain a the project logos and some other nice images. 


-   [Logo Small]({{ site.baseurl }}/images/logo389.png)
-   [Wallpaper 16:9 svg]({{ site.baseurl }}/images/389-logo-wallpaper-1080p.svg)

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />These <span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/StillImage" rel="dct:type">works</span> are licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
