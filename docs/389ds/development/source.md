---
title: "Source"
---

# Directory Server Source Code
------------------------------

{% include toc.md %}

These are the sources used by the directory server which are provided by the project (as opposed to third party sources like the Mozilla components, berkeley db, etc.).

[All the source tarballs]({{ site.binaries_url }}/binaries/)

All of the source is now in git. The git module given below is a sub-directory of the base git URL **git@pagure.io/389-ds-base.git** - so for the base directory server, the full git URL is **https://pagure.io/389-ds-base.git**

The idm-console-framework is not under 389/ it is at **git://git@pagure.io/idm-console-framework.git**

The source code was produced by first doing a git clone to get the repository, then a git archive to produce the source tarball

    git clone https://git@pagure.io/389-ds-base.git

    git archive --prefix=PKGNAME/ TAG | bzip2 > PKGNAME.tar.bz2


### python-lib389 1.0.4

|Source tarball|git module|git tag|More Info|SHA256SUM|
|--------------|----------|-------|---------|-------|
|[python-lib389-1.0.4.tar.bz2]({{ site.binaries_url }}/binaries/python-lib389-1.0.4.tar.bz2)|lib389.git|python-lib389-1.0.4|[lib389](http://www.port389.org/docs/389ds/FAQ/upstream-test-framework.html)|6b22fd9277adebd595e30ac614741d21f8df91d4e9e303c3c5fa3044609060bb|


### 389 Admin Server and Console packges 1.1.46

|Source tarball|git module|git tag|More Info|SHA1SUM|
|--------------|----------|-------|---------|-------|
|[389-admin.1.1.46.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-1.1.46.tar.bz2)|admin.git|389-admin-1.1.46|[Admin](../administration/adminserver.html)|735c51c0f19e448fbe9f552893ee4f9297420831|
|[389-adminutil.1.1.23.tar.bz2]({{ site.binaries_url }}/binaries/389-adminutil-1.1.23.tar.bz2)|adminutil.git|389-adminutil-1.1.23|[Adminutil](../administration/adminutil.html)|daf72628b97337ad2b48e8753f2bc7b01a4482c0|
|[389-console.1.1.18.tar.bz2]({{ site.binaries_url }}/binaries/389-console-1.1.18.tar.bz2)|console.git|389-admin-1.1.45|[Building Console](buildingconsole.html)|ad6929bc9391d7b725aa8246fce5cc22225829b3|
|[389-admin-console.1.1.12.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-console-1.1.12.tar.bz2)|admin-console.git|389-admin-console-1.1.12|[Building Console](buildingconsole.html)|ecfce08e40760f9b8ed4e3b0aa90d7e026d761f9|
|[389-ds-console-1.2.16.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-console-1.2.16.tar.bz2)|ds-console.git|389-ds-console-1.2.16|[Building Console](buildingconsole.html)|1c7977a6720e77ccc26440c54672b729f9a8820d|
|[idm-console-framework-1.1.17.tar.bz2]({{ site.binaries_url }}/binaries/idm-console-framework-1.1.17.tar.bz2)|idm-console-framework.git|idm-console-framework-1.1.17|[Building Console](buildingconsole.html)|abaa10be90f51ed61e4d16348eee7706fda19df1|

### EPEL6 packages

|[389-admin.1.1.43.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-1.1.43.tar.bz2)|admin.git|389-admin-1.1.43|[Admin](../administration/adminserver.html)|3d931830ce832b7e0f820689ca30e5996b873f75|
|[389-console-1.1.17.tar.bz2]({{ site.binaries_url }}/binaries/389-console-1.1.17.tar.bz2)|console.git|389-console-1.1.17|[Building Console](buildingconsole.html)|b63c5c53936752e55ba205ba827af7cc96658cbb|
|[389-admin-console-1.1.11.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-console-1.1.11.tar.bz2)|admin-console.git|389-admin-console-1.1.11|[Building Console](buildingconsole.html)|852a1c121923137b9048b7e498b7f03965cc0d3b|
|[idm-console-framework-1.1.15.tar.bz2]({{ site.binaries_url }}/binaries/idm-console-framework-1.1.15.tar.bz2)|idm-console-framework.git|idm-console-framework-1.1.15|[Building Console](buildingconsole.html)|86ca70b34bba1ceffb206cd945a5d077544a83f7|

### 389 Directory Server 1.4.0

|Source tarball|git module|git tag|More Info|SHA256SUM|
|--------------|----------|-------|---------|-------|
|[389-ds-base-1.4.0.8.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.4.0.8.tar.bz2)|389-ds-base.git|389-ds-base-1.4.0.8|[Building](building.html)|26ccc00b9f436c33517e8493442c8ee806bced59784ed3abed9d6904559bc990|
|[389-ds-base-1.4.0.7.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.4.0.7.tar.bz2)|389-ds-base.git|389-ds-base-1.4.0.7|[Building](building.html)|ca76e2c4b8a83d82bd80499542e8fdf03c50952342cc4c0bd58dbf4503f2351a|
|[389-ds-base-1.4.0.6.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.4.0.6.tar.bz2)|389-ds-base.git|389-ds-base-1.4.0.6|[Building](building.html)|a9f9a3364b1f167cc4f6da353e31f8efbb2300f0e432c11616db4bba61103192|
|[389-ds-base-1.4.0.5.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.4.0.5.tar.bz2)|389-ds-base.git|389-ds-base-1.4.0.5|[Building](building.html)|4a2e6359abfc4c23ef5f13374bdb9c27d7a2d026a1a9f194d2562dc91d641448|
|[389-ds-base-1.4.0.4.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.4.0.4.tar.bz2)|389-ds-base.git|389-ds-base-1.4.0.4|[Building](building.html)|a0ea02fc3f7f808dcf1eda4a35df2cfc639e035283c2d6ce03c010b2794434e1|
|[389-ds-base-1.4.0.3.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.4.0.3.tar.bz2)|389-ds-base.git|389-ds-base-1.4.0.3|[Building](building.html)|7aeb387b8df4fa06c66baacc09f05d7fa7b9a0f69350a41576f095a2b12ea180|
|[389-ds-base-1.4.0.2.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.4.0.2.tar.bz2)|389-ds-base.git|389-ds-base-1.4.0.2|[Building](building.html)|65bdf20ccdcb949c01ca4e0ce0db84313f97cee2e2020714bff0eb50595a487c|
|[389-ds-base-1.4.0.1.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.4.0.1.tar.bz2)|389-ds-base.git|389-ds-base-1.4.0.1|[Building](building.html)|fa4ea2ab3467ed14e8259d40dc2e5c2b0d1d42269929ff0a72ea7199043c0f1e|
|[389-ds-base-1.4.0.0.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.4.0.0.tar.bz2)|389-ds-base.git|389-ds-base-1.4.0.0|[Building](building.html)|d557e44959ec9e11f08350c4d2a5753b05a2b1582c399a640f3359bca539ca79|


### 389 Directory Serfer 1.3.7

|Source tarball|git module|git tag|More Info|SHA256SUM|
|--------------|----------|-------|---------|-------|
|[389-ds-base-1.3.7.9.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.3.7.9.tar.bz2)|389-ds-base.git|389-ds-base-1.3.7.9|[Building](building.html)|fe9e7bee67ff6ce8b41d7e7c74dae79bd69711bcb488fe8c226e218357331e37|
|[389-ds-base-1.3.7.8.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.3.7.8.tar.bz2)|389-ds-base.git|389-ds-base-1.3.7.8|[Building](building.html)|7f7bd56c05059add1c386fd48bad1324756b142b60c3ba0364736261aba200a0|
|[389-ds-base-1.3.7.7.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.3.7.7.tar.bz2)|389-ds-base.git|389-ds-base-1.3.7.7|[Building](building.html)|6353f1e7578daa18a3816fd5028c5b6df4f29d6ce43be6b524316f6f8e3f10a3|
|[389-ds-base-1.3.7.6.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.3.7.6.tar.bz2)|389-ds-base.git|389-ds-base-1.3.7.6|[Building](building.html)|7236e71489b832f9e13d2b2f8b5a93060dc0e0ff92fb35a0d39641bae020a769|
|[389-ds-base-1.3.7.5.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.3.7.5.tar.bz2)|389-ds-base.git|389-ds-base-1.3.7.5|[Building](building.html)|007ce281d2961ed7139d90c6fe38d7fbe532d7b46589bca1ec7465d57229dfc9|
|[389-ds-base-1.3.7.4.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.7.4.tar.bz2)|389-ds-base.git|389-ds-base-1.3.7.4|[Building](building.html)|bc5021b37c240a848f9567b31dc91ee7e8dea564360cceedf42a962a910aee5e|
|[389-ds-base-1.3.7.3.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.7.3.tar.bz2)|389-ds-base.git|389-ds-base-1.3.7.3|[Building](building.html)|ccbbee067142a8c7e005a57e6b0eb2df8b7581b02ccce4e6d4c86b89b71f1d69|
|[389-ds-base-1.3.7.2.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.7.2.tar.bz2)|389-ds-base.git|389-ds-base-1.3.7.2|[Building](building.html)|dbbf2dcc76a6cf2527a1a59f3bf4315717e233e321a9d3ee1cdf67e17ab33e48|
|[389-ds-base-1.3.7.1.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.7.1.tar.bz2)|389-ds-base.git|389-ds-base-1.3.7.1|[Building](building.html)|3f5b85988f2d5c17c4c3f021593863f1798a32b43d594c08163a06bf3d5ed2fe|


### 389 Directory Server 1.3.6

|Source tarball|git module|git tag|More Info|SHA256SUM|
|--------------|----------|-------|---------|-------|
|[389-ds-base-1.3.6.13.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.3.6.13.tar.bz2)|389-ds-base.git|389-ds-base-1.3.6.13|[Building](building.html)|524744dc5afa37409e22684a71f603dec094f7b37d9d053390eff1617b278f61|
|[389-ds-base-1.3.6.12.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.3.6.12.tar.bz2)|389-ds-base.git|389-ds-base-1.3.6.12|[Building](building.html)|746eaf134d4dd2bdf51ee3d2a05a6f71e5e2fcbcd31f22892aa714d0b1d7f454|
|[389-ds-base-1.3.6.11.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.3.6.11.tar.bz2)|389-ds-base.git|389-ds-base-1.3.6.11|[Building](building.html)|fb931af243d8764349e609b9893dde05886cee8d53708beb0e8130a1ef70e603|
|[389-ds-base-1.3.6.10.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.3.6.10.tar.bz2)|389-ds-base.git|389-ds-base-1.3.6.10|[Building](building.html)|866ac60a4c38184505a97762132f77800525b136fd071c19cf054b7d0b4bad0e|
|[389-ds-base-1.3.6.9.tar.bz2](https://releases.pagure.org/389-ds-base/389-ds-base-1.3.6.9.tar.bz2)|389-ds-base.git|389-ds-base-1.3.6.9|[Building](building.html)|246b533b65d7202635c60afb625244645ecb15ec1d0fe0f882a36308989a23ec|
|[389-ds-base-1.3.6.8.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.6.8.tar.bz2)|389-ds-base.git|389-ds-base-1.3.6.8|[Building](building.html)|447997455d0b9cf97c9bb86f23066d119c73c3a12b473fa45b4f1a8299d50e8a|
|[389-ds-base-1.3.6.7.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.6.7.tar.bz2)|389-ds-base.git|389-ds-base-1.3.6.7|[Building](building.html)|d6a8a4dbe1ebd30eff2ad20f550fe2e1b2673ca632cbfbee46baaff2671062db|
|[389-ds-base-1.3.6.6.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.6.6.tar.bz2)|389-ds-base.git|389-ds-base-1.3.6.6|[Building](building.html)|d1f2e3f8a44bb035b2724aa2dc5c7d7b751fbe305f935a4377dea821dad1be94|
|[389-ds-base-1.3.6.5.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.6.5.tar.bz2)|389-ds-base.git|389-ds-base-1.3.6.5|[Building](building.html)|a0bcdcb6231399c507a7d28c3282fe2bb226bea39ee1a7b2604aeae88059a797|
|[389-ds-base-1.3.6.4.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.6.4.tar.bz2)|389-ds-base.git|389-ds-base-1.3.6.4|[Building](building.html)|e370270391d9e4bac4eb969380f76fbc715886a8f0b156433fee932d2701fbedd8f0460369a2878dd8f134ac5f35393ea2ea76b25cb24e91b744c1de2af3d879|
|[389-ds-base-1.3.6.3.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.6.3.tar.bz2)|389-ds-base.git|389-ds-base-1.3.6.3|[Building](building.html)|bd45bc424d58e91d0855f075614ff3cdd99be9b517789743c44f6d6a025aecce|
|[389-ds-base-1.3.6.1.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.6.1.tar.bz2)|389-ds-base.git|389-ds-base-1.3.6.1|[Building](building.html)|a814776ce153dd75e86ebcc7bbf4106ef1ee7492bcccf41c2eb5b984de31a48a|
|[svrcore-4.1.2.tar.bz2]({{ site.binaries_url }}/binaries/svrcore-4.1.2.tar.bz2)|svrcore.git|4.1.2|[Building](building-svrcore.html)|67e51a868c8dc2ddbf5661ecb0a07dea7721a9ed99f6261cedd3351bfc4cd023|


### 389 Directory Server 1.3.5

|Source tarball|git module|git tag|More Info|SHA1SUM/SHA256SUM|
|--------------|----------|-------|---------|-------|

|[389-ds-base-1.3.5.19.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.5.19.tar.bz2)|389-ds-base.git|389-ds-base-1.3.5.19|[Building](building.html)|ad55aadd4155cabdb7cc66dbca3bbe43faf865750da01032c9a1f8ed3a2136e4|
|[389-ds-base-1.3.5.18.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.5.18.tar.bz2)|389-ds-base.git|389-ds-base-1.3.5.18|[Building](building.html)|cf86bbeb21096d3d5dc51398790a74ed8c8f7aefbb54c233f4962b0c99216997|
|[389-ds-base-1.3.5.17.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.5.17.tar.bz2)|389-ds-base.git|389-ds-base-1.3.5.17|[Building](building.html)|5b96b19cea7dc80c64eaade31127d04c228f7e4dc1999ec19b341cf080ee4570757c84e8dae151c2cb3bcebe1398d50238d74ca362ce07fceafcb66fba590833|
|[389-ds-base-1.3.5.16.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.5.16.tar.bz2)|389-ds-base.git|389-ds-base-1.3.5.16|[Building](building.html)|29cdd0066447a0de9b5455444a2020a9d1a0aca8|
|[389-ds-base-1.3.5.15.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.5.15.tar.bz2)|389-ds-base.git|389-ds-base-1.3.5.15|[Building](building.html)|856753525d074c36acdba087880f68edb0236211|
|[389-ds-base-1.3.5.14.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.5.14.tar.bz2)|389-ds-base.git|389-ds-base-1.3.5.14|[Building](building.html)|9c81ce4093790dfa31ca9eba1ebbf10f024e7684|
|[389-ds-base-1.3.5.13.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.5.13.tar.bz2)|389-ds-base.git|389-ds-base-1.3.5.13|[Building](building.html)|cef01f8347c3164f14089b4f647b9e986ef667cd|
|[nunc-stans-0.1.8.tar.bz2]({{ site.binaries_url }}/binaries/nunc-stans-0.1.8.tar.bz2)|nunc-stans.git|0.1.8|[Building](building.html)|835c9788650d1b9ef0896c267b06b9e529612835|
|[svrcore-4.1.2.tar.bz2]({{ site.binaries_url }}/binaries/svrcore-4.1.2.tar.bz2)|svrcore.git|4.1.2|[Building](building.html)|699db1b2294e7d15c8f576037fc5ff9bc6d8e001|

### 389 Directory Server 1.3.4

389-ds-base uses git repo https://pagure.io/389-ds-base.git branch 389-ds-base-1.3.4 (branched 19-Jun-2015)

|Source tarball|git module|git tag|More Info|SHA1SUM|
|--------------|----------|-------|---------|-------|
|[389-ds-base-1.3.4.15.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.4.15.tar.bz2)|ds.git|389-ds-base-1.3.4.15|[Building](building.html)|d453f6a982253d96efa4f616089b600331d5c740|
|[389-ds-base-1.3.4.14.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.4.14.tar.bz2)|ds.git|389-ds-base-1.3.4.14|[Building](building.html)|3c45f7a97b5c8c5475370df9efc8797a7346ff44|
|[nunc-stans-0.1.5.tar.bz2]({{ site.binaries_url }}/binaries/nunc-stans-0.1.5.tar.bz2)|nunc-stans.git|0.1.5|[Building](building.html)|7e52309f61c38b241fcdaf0284559d683f3ba700|
|[389-admin.1.1.42.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-1.1.42.tar.bz2)|admin.git|389-admin-1.1.42|[Admin](../administration/adminserver.html)|3d931830ce832b7e0f820689ca30e5996b873f75|
|[389-adminutil-1.1.22.tar.bz2]({{ site.binaries_url }}/binaries/389-adminutil-1.1.22.tar.bz2)|adminutil.git|389-adminutil-1.1.22|[AdminUtil](../administration/adminutil.html)|ee337a293409b9682f68797bf200ef4a7e14c3e1|
|[389-console-1.1.9.tar.bz2]({{ site.binaries_url }}/binaries/389-console-1.1.9.tar.bz2)|console.git|389-console-1.1.9|[Building Console](buildingconsole.html)|bcc15330156beab1dab57cedef838f8ec5b26988|
|[389-ds-console-1.2.12.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-console-1.2.12.tar.bz2)|ds-console.git|389-ds-console-1.2.12|[Building Console](buildingconsole.html)|e71273413d9375d2b0713f18f69d48ad859603b7|
|[389-admin-console-1.1.10.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-console-1.1.10.tar.bz2)|admin-console.git|389-admin-console-1.1.10|[Building Console](buildingconsole.html)|3f79901cb5457220e34480032cfcc14879dbbb68|
|[idm-console-framework-1.1.14.tar.bz2]({{ site.binaries_url }}/binaries/idm-console-framework-1.1.14.tar.bz2)|idm-console-framework.git|idm-console-framework-1.1.14|[Building Console](buildingconsole.html)|fd6be1df38d8c1182b16b5f9d603860ce8cc1c9c|

### 389 Directory Server 1.3.3

389-ds-base uses git repo 389/ds.git branch 389-ds-base-1.3.3 (branched 21-AUG-2014)

|Source tarball|git module|git tag|More Info|SHA1SUM|
|--------------|----------|-------|---------|-------|
|[389-ds-base-1.3.3.14.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.3.14.tar.bz2)|ds.git|389-ds-base-1.3.3.14|[Building](building.html)|4b5d6db460b903a5073dc3e6086dec199f839049|
|[389-admin.1.1.42.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-1.1.42.tar.bz2)|admin.git|389-admin-1.1.42|[Admin](../administration/adminserver.html)|3d931830ce832b7e0f820689ca30e5996b873f75|
|[389-adminutil-1.1.22.tar.bz2]({{ site.binaries_url }}/binaries/389-adminutil-1.1.22.tar.bz2)|adminutil.git|389-adminutil-1.1.22|[AdminUtil](../administration/adminutil.html)|ee337a293409b9682f68797bf200ef4a7e14c3e1|
|[389-console-1.1.9.tar.bz2]({{ site.binaries_url }}/binaries/389-console-1.1.9.tar.bz2)|console.git|389-console-1.1.9|[Building Console](buildingconsole.html)|bcc15330156beab1dab57cedef838f8ec5b26988|
|[389-ds-console-1.2.12.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-console-1.2.12.tar.bz2)|ds-console.git|389-ds-console-1.2.12|[Building Console](buildingconsole.html)|e71273413d9375d2b0713f18f69d48ad859603b7|
|[389-admin-console-1.1.10.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-console-1.1.10.tar.bz2)|admin-console.git|389-admin-console-1.1.10|[Building Console](buildingconsole.html)|3f79901cb5457220e34480032cfcc14879dbbb68|
|[idm-console-framework-1.1.14.tar.bz2]({{ site.binaries_url }}/binaries/idm-console-framework-1.1.14.tar.bz2)|idm-console-framework.git|idm-console-framework-1.1.14|[Building Console](buildingconsole.html)|fd6be1df38d8c1182b16b5f9d603860ce8cc1c9c|

### 389 Directory Server 1.3.2

389-ds-base uses git repo 389/ds.git branch 389-ds-base-1.3.2 (branched 1-OCT-2013)

|Source tarball|git module|git tag|More Info|SHA1SUM|
|--------------|----------|-------|---------|-------|
|[389-ds-base-1.3.2.27.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.2.27.tar.bz2)|ds.git|389-ds-base-1.3.2.27|[Building](building.html)|dc6bcbd97923dec7ff13a6437a07246723b6feff|
|[389-dsgw-1.1.11.tar.bz2]({{ site.binaries_url }}/binaries/389-dsgw-1.1.11.tar.bz2)|dsgw.git|389-dsgw-1.1.11|[DSGW\_Building](../administration/dsgw-building.html)|6a2b94be7d4f0079dbe5e84d720ff8f5e1779aba|
|[389-admin-1.1.38.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-1.1.38.tar.bz2)|admin.git|389-admin-1.1.38|[Admin](../administration/adminserver.html)|52f43945a6786f83009e5745c98b2c24f42f2797|
|[389-adminutil-1.1.21.tar.bz2]({{ site.binaries_url }}/binaries/389-adminutil-1.1.21.tar.bz2)|adminutil.git|389-adminutil-1.1.21|[AdminUtil](../administration/adminutil.html)|7a78b262d966897e78a3c94f1ae9e7126ea53f9f|
|[389-console-1.1.9.tar.bz2]({{ site.binaries_url }}/binaries/389-console-1.1.9.tar.bz2)|console.git|389-console-1.1.9|[Building Console](buildingconsole.html)|bcc15330156beab1dab57cedef838f8ec5b26988|
|[389-ds-console-1.2.10.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-console-1.2.10.tar.bz2)|ds-console.git|389-ds-console-1.2.10|[Building Console](buildingconsole.html)|c4f38cd421ffcc8b26fd841e4e45096bbaf21451|
|[389-admin-console-1.1.10.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-console-1.1.10.tar.bz2)|admin-console.git|389-admin-console-1.1.10|[Building Console](buildingconsole.html)|3f79901cb5457220e34480032cfcc14879dbbb68|
|[idm-console-framework-1.1.9.tar.bz2]({{ site.binaries_url }}/binaries/idm-console-framework-1.1.9.tar.bz2)|idm-console-framework.git|idm-console-framework-1.1.9|[Building Console](buildingconsole.html)|38f79c7248106738ed10beca936eb85b40249a8f|

### 389 Directory Server 1.3.1

389-ds-base uses git repo 389/ds.git branch 389-ds-base-1.3.1 (branched 13-FEB-2013)

|Source tarball|git module|git tag|More Info|SHA1SUM|
|--------------|----------|-------|---------|-------|
|[389-ds-base-1.3.1.22.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.1.22.tar.bz2)|ds.git|389-ds-base-1.3.1.22|[Building](building.html)|671536bc70633e802b401c69d76da06e09e04ae0|
|[389-adminutil-1.1.18.tar.bz2]({{ site.binaries_url }}/binaries/389-adminutil-1.1.18.tar.bz2)|adminutil.git|389-adminutil-1.1.18|[AdminUtil](../administration/adminutil.html)|054a9e06e91e1e0d8f88903cbcf8e7ab8b270589|

### 389 Directory Server 1.3.0

389-ds-base uses git repo 389/ds.git branch 389-ds-base-1.3.0 (branched 11-DEC-2012)

|Source tarball|git module|git tag|More Info|SHA1SUM|
|--------------|----------|-------|---------|-------|
|[389-ds-base-1.3.0.9.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.0.9.tar.bz2)|ds.git|389-ds-base-1.3.0.9|[Building](building.html)|45d9ccdaac75e7702de68d0972a27d39fefc67e9|
|[389-ds-base-1.3.0.3.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.3.0.3.tar.bz2)|ds.git|389-ds-base-1.3.0.3|[Building](building.html)|39f2b96bd6d6760af07780157efecc661d0e88c0|
|[389-admin-1.1.31.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-1.1.31.tar.bz2)|admin.git|389-admin-1.1.31|[AdminServer](../administration/adminserver.html)|bbfc6313db39bb55fa1cbd03fca8fffdcff286ae|
|[389-adminutil-1.1.18.tar.bz2]({{ site.binaries_url }}/binaries/389-adminutil-1.1.18.tar.bz2)|adminutil.git|389-adminutil-1.1.18|[AdminUtil](../administration/adminutil.html)|054a9e06e91e1e0d8f88903cbcf8e7ab8b270589|
|[389-dsgw-1.1.10.tar.bz2]({{ site.binaries_url }}/binaries/389-dsgw-1.1.10.tar.bz2)|dsgw.git|389-dsgw-1.1.10|[DSGW\_Building](../administration/dsgw-building.html)|f147769e82187b570eb3e39b3a9fb1572bdd4512|
|[winsync-1.1.4.tar.bz2]({{ site.binaries_url }}/binaries/winsync-1.1.4.tar.bz2)|winsync.git|winsync-1.1.4|[WindowsSync](../howto/howto-windowssync.html)|3e45d315038d0694d7f801bd4911e3f1f524191f|
|[389-console-1.1.7.tar.bz2]({{ site.binaries_url }}/binaries/389-console-1.1.7.tar.bz2)|console.git|389-console-1.1.7|[WindowsSync](../howto/howto-windowsconsole.html|87ae48c131b2964f9dac97e011a8a8fb61d3a8a4|
|[idm-console-framework-1.1.7.tar.bz2]({{ site.binaries_url }}/binaries/idm-console-framework-1.1.7.tar.bz2)|idm-console-framework.git|idm-console-framework-1.1.7|[buildingconsole.html](buildingconsole.html)|2081dea597c2fe0078a8a8f4047884cb1e02e470|
|[389-ds-console-1.2.7.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-console-1.2.7.tar.bz2)|ds-console.git|389-ds-console-1.2.7|[DirectoryConsole](buildingconsole.html#ds-console)|21ed7ce7b2a2c0a529d251bbd33435d60a93a4fa|
|[389-admin-console-1.1.8.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-console-1.1.8.tar.bz2)|admin-console.git|389-admin-console-1.1.8|[AdminConsole](buildingconsole.html#admin-console)|8e093715b215e64ae9b307bc96df55d2bd496da8|

### 389 Directory Server 1.2.11

389-ds-base uses git repo 389/ds.git branch 389-ds-base-1.2.11

|Source tarball|git module|git tag|More Info|SHA1SUM|
|--------------|----------|-------|---------|-------|
|[389-ds-base-1.2.11.29.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.2.11.29.tar.bz2)|ds.git|389-ds-base-1.2.11.29|[Building](building.html)|ad392648f8dfa66c8a6d9d6843e1d10a3d518ae6|
|[389-admin-1.1.30.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-1.1.30.tar.bz2)|admin.git|389-admin-1.1.30|[AdminServer](../administration/adminserver.html)|971fb47a5d97cd32b6820f0f4cb99c196165dd0f|
|[389-adminutil-1.1.15.tar.bz2]({{ site.binaries_url }}/binaries/389-adminutil-1.1.15.tar.bz2)|adminutil.git|389-adminutil-1.1.15|[AdminUtil](../administration/adminutil.html)|bbf4219b55bb1af0a76bb75bb16af4121b36f4de|
|[389-dsgw-1.1.10.tar.bz2]({{ site.binaries_url }}/binaries/389-dsgw-1.1.10.tar.bz2)|dsgw.git|389-dsgw-1.1.10|[DSGW\_Building](../administration/dsgw-building.html)|f147769e82187b570eb3e39b3a9fb1572bdd4512|
|[winsync-1.1.4.tar.bz2]({{ site.binaries_url }}/binaries/winsync-1.1.4.tar.bz2)|winsync.git|winsync-1.1.4|[WindowsSync](../howto/howto-windowssync.html|3e45d315038d0694d7f801bd4911e3f1f524191f|
|[389-console-1.1.7.tar.bz2]({{ site.binaries_url }}/binaries/389-console-1.1.7.tar.bz2)|console.git|389-console-1.1.7|[WindowsSync](../howto/howto-windowsconsole.html|87ae48c131b2964f9dac97e011a8a8fb61d3a8a4|
|[idm-console-framework-1.1.7.tar.bz2]({{ site.binaries_url }}/binaries/idm-console-framework-1.1.7.tar.bz2)|idm-console-framework.git|idm-console-framework-1.1.7|[buildingconsole.html](buildingconsole.html)|2081dea597c2fe0078a8a8f4047884cb1e02e470|
|[389-ds-console-1.2.6.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-console-1.2.6.tar.bz2)|ds-console.git|389-ds-console-1.2.6|[DirectoryConsole](buildingconsole.html#ds-console)|adc763187f6b2e7f9f347b930276ab5712eb7807|
|[389-admin-console-1.1.8.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-console-1.1.8.tar.bz2)|admin-console.git|389-admin-console-1.1.8|[AdminConsole](buildingconsole.html#admin-console)|8e093715b215e64ae9b307bc96df55d2bd496da8|

### 389 Directory Server 1.2.10

389-ds-base uses git repo 389/ds.git branch 389-ds-base-1.2.10

|Source tarball|git module|git tag|More Info|SHA1SUM|
|--------------|----------|-------|---------|-------|
|[389-ds-base-1.2.10.14.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.2.10.14.tar.bz2)|ds.git|389-ds-base-1.2.10.14|[Building](building.html)|8de0e6c9d77041d48927200c42f5400645672db1|
|[389-admin-1.1.29.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-1.1.29.tar.bz2)|admin.git|389-admin-1.1.29|[AdminServer](../administration/adminserver.html)|6cdb023dadd0862327fd09f06f6a51454ff8672c|
|[389-adminutil-1.1.15.tar.bz2]({{ site.binaries_url }}/binaries/389-adminutil-1.1.14.tar.bz2)|adminutil.git|389-adminutil-1.1.15|[AdminUtil](../administration/adminutil.html)|bbf4219b55bb1af0a76bb75bb16af4121b36f4de|
|[389-dsgw-1.1.9.tar.bz2]({{ site.binaries_url }}/binaries/389-dsgw-1.1.9.tar.bz2)|dsgw.git|389-dsgw-1.1.9|[DSGW\_Building](../administration/dsgw-building.html)|8bf25eeda80ec9fb15c53564dbaa32e5d2c7deff|
|[winsync-1.1.4.tar.bz2]({{ site.binaries_url }}/binaries/winsync-1.1.4.tar.bz2)|winsync.git|winsync-1.1.4|[WindowsSync](../howto-windowssync.html)|3e45d315038d0694d7f801bd4911e3f1f524191f|
|[389-console-1.1.7.tar.bz2]({{ site.binaries_url }}/binaries/389-console-1.1.7.tar.bz2)|console.git|389-console-1.1.7|[WindowsSync](../howto/howto-windowsconsole.html|87ae48c131b2964f9dac97e011a8a8fb61d3a8a4|
|[idm-console-framework-1.1.7.tar.bz2]({{ site.binaries_url }}/binaries/idm-console-framework-1.1.7.tar.bz2)|idm-console-framework.git|idm-console-framework-1.1.7|[buildingconsole.html](buildingconsole.html)|2081dea597c2fe0078a8a8f4047884cb1e02e470|
|[389-ds-console-1.2.6.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-console-1.2.6.tar.bz2)|ds-console.git|389-ds-console-1.2.6|[DirectoryConsole](buildingconsole.html#ds-console)|adc763187f6b2e7f9f347b930276ab5712eb7807|
|[389-admin-console-1.1.8.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-console-1.1.8.tar.bz2)|admin-console.git|389-admin-console-1.1.8|[AdminConsole](buildingconsole.html#admin-console)|8e093715b215e64ae9b307bc96df55d2bd496da8|

### 389 Directory Server 1.2.9

389-ds-base uses git repo 389/ds.git branch 389-ds-base-1.2.9

|Source tarball|git module|git tag|More Info|SHA1SUM|
|--------------|----------|-------|---------|-------|
|[389-ds-base-1.2.9.9.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.2.9.9.tar.bz2)|ds.git|389-ds-base-1.2.9.9|[Building](building.html)|d61a7284eafe5984a38e332445049d15679ed14e|
|[389-admin-1.1.23.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-1.1.23.tar.bz2)|admin.git|389-admin-1.1.23|[AdminServer](../administration/adminserver.html)|b3013f3ce833f5dae8ec33f881f46a064f4d1d3d|
|[389-adminutil-1.1.14.tar.bz2]({{ site.binaries_url }}/binaries/389-adminutil-1.1.14.tar.bz2)|adminutil.git|389-adminutil-1.1.14|[AdminUtil](../administration/adminutil.html)|b6af0f12cdeda2d1188a6c6c1d7851da60ad4331|
|[389-dsgw-1.1.7.tar.bz2]({{ site.binaries_url }}/binaries/389-dsgw-1.1.7.tar.bz2)|dsgw.git|389-dsgw-1.1.7|[DSGW\_Building](../administration/dsgw-building.html)|0eb4e05d7ae763395a9338b0a76f441be51612e7|
|[winsync-1.1.4.tar.bz2]({{ site.binaries_url }}/binaries/winsync-1.1.4.tar.bz2)|winsync.git|winsync-1.1.4|[WindowsSync](../howto/howto-windowssync.html|3e45d315038d0694d7f801bd4911e3f1f524191f|
|[389-console-1.1.7.tar.bz2]({{ site.binaries_url }}/binaries/389-console-1.1.7.tar.bz2)|console.git|389-console-1.1.7|[WindowsSync](../howto/howto-windowsconsole.html|87ae48c131b2964f9dac97e011a8a8fb61d3a8a4|
|[idm-console-framework-1.1.7.tar.bz2]({{ site.binaries_url }}/binaries/idm-console-framework-1.1.7.tar.bz2)|idm-console-framework.git|idm-console-framework-1.1.7|[buildingconsole.html](buildingconsole.html)|2081dea597c2fe0078a8a8f4047884cb1e02e470|
|[389-ds-console-1.2.6.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-console-1.2.6.tar.bz2)|ds-console.git|389-ds-console-1.2.6|[DirectoryConsole](buildingconsole.html#ds-console)|adc763187f6b2e7f9f347b930276ab5712eb7807|
|[389-admin-console-1.1.8.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-console-1.1.8.tar.bz2)|admin-console.git|389-admin-console-1.1.8|[AdminConsole](buildingconsole.html#admin-console)|8e093715b215e64ae9b307bc96df55d2bd496da8|

### 389 Directory Server 1.2.8

|Source tarball|git module|git tag|More Info|SHA1SUM|
|--------------|----------|-------|---------|-------|
|[389-ds-base-1.2.8.3.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.2.8.3.tar.bz2)|ds.git|389-ds-base-1.2.8.3|[Building](building.html)|87f1f8ec0044f4b1766b2b65b34f4e14d9d0d41d|
|[389-admin-1.1.16.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-1.1.16.tar.bz2)|admin.git|389-admin-1.1.16|[AdminServer](../administration/adminserver.html)|e2facc231d1475b218321b7dbdb04d8f9b6ebacb|
|[389-adminutil-1.1.13.tar.bz2]({{ site.binaries_url }}/binaries/389-adminutil-1.1.13.tar.bz2)|adminutil.git|389-adminutil-1.1.13|[AdminUtil](../administration/adminutil.html)|1de90fc408b0046aeb346fad7e2251f10e07024a|
|[389-dsgw-1.1.6.tar.bz2]({{ site.binaries_url }}/binaries/389-dsgw-1.1.6.tar.bz2)|dsgw.git|389-dsgw-1.1.6|[DSGW\_Building](../administration/dsgw-building.html)|2e18c7b3ccb7c98b68917538c2a75eb445b734db|
|[winsync-1.1.4.tar.bz2]({{ site.binaries_url }}/binaries/winsync-1.1.4.tar.bz2)|winsync.git|winsync-1.1.4|[WindowsSync](../howto/howto-windowssync.html|3e45d315038d0694d7f801bd4911e3f1f524191f|
|[389-console-1.1.6.tar.bz2]({{ site.binaries_url }}/binaries/389-console-1.1.6.tar.bz2)|console.git|389-console-1.1.6|[WindowsSync](../howto/howto-windowsconsole.html|06f7128bc86d1429c6fd0a920ecbb0bac9799206|
|[idm-console-framework-1.1.7.tar.bz2]({{ site.binaries_url }}/binaries/idm-console-framework-1.1.7.tar.bz2)|console(CVS)|FedoraConsoleFramework\_1\_1\_7(CVS)|[buildingconsole.html](buildingconsole.html)|f64814028eb4abc8d7fadac794d52f1b9d32de99|
|[389-ds-console-1.2.5.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-console-1.2.5.tar.bz2)|ds-console.git|389-ds-console-1.2.5|[DirectoryConsole](buildingconsole.html#ds-console)|d3eafbec8e7b71f05baa3a9e64ba31692ed6daf8|
|[389-admin-console-1.1.7.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-console-1.1.7.tar.bz2)|admin-console.git|389-admin-console-1.1.7|[AdminConsole](buildingconsole.html#admin-console)|917db7c8b6f4390cbe688966826ac499d6d6cd75|

### 389 Directory Server 1.2.7

|Source tarball|git module|git tag|More Info|SHA1SUM|
|--------------|----------|-------|---------|-------|
|[389-ds-base-1.2.7.5.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.2.7.5.tar.bz2)|ds.git|389-ds-base-1.2.7.5|[Building](building.html)|5277c8b26ab45c4399a836de4c4c0294b6b4de2b|
|[389-admin-1.1.14.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-1.1.14.tar.bz2)|admin.git|389-admin-1.1.14|[AdminServer](../administration/adminserver.html)|8379b955de459e0efcb1207f8da0881fcd6d9964|
|[389-adminutil-1.1.13.tar.bz2]({{ site.binaries_url }}/binaries/389-adminutil-1.1.13.tar.bz2)|adminutil.git|389-adminutil-1.1.13|[AdminUtil](../administration/adminutil.html)|1de90fc408b0046aeb346fad7e2251f10e07024a|
|[389-dsgw-1.1.6.tar.bz2]({{ site.binaries_url }}/binaries/389-dsgw-1.1.6.tar.bz2)|dsgw.git|389-dsgw-1.1.6|[DSGW\_Building](../administration/dsgw-building.html)|2e18c7b3ccb7c98b68917538c2a75eb445b734db|
|[winsync-1.1.4.tar.bz2]({{ site.binaries_url }}/binaries/winsync-1.1.4.tar.bz2)|winsync.git|winsync-1.1.4|[WindowsSync](../howto/howto-windowssync.html|3e45d315038d0694d7f801bd4911e3f1f524191f|
|[389-console-1.1.6.tar.bz2]({{ site.binaries_url }}/binaries/389-console-1.1.6.tar.bz2)|console.git|389-console-1.1.6|[WindowsSync](../howto/howto-windowsconsole.html|06f7128bc86d1429c6fd0a920ecbb0bac9799206|
|[idm-console-framework-1.1.5.tar.bz2]({{ site.binaries_url }}/binaries/idm-console-framework-1.1.5.tar.bz2)|console(CVS)|FedoraConsoleFramework\_1\_1\_5(CVS)|[buildingconsole.html](buildingconsole.html)|15f1d2af4cac986c6caad39f4ed02191169fcb42|
|[389-ds-console-1.2.3.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-console-1.2.3.tar.bz2)|ds-console.git|389-ds-console-1.2.3|[DirectoryConsole](buildingconsole.html#ds-console)|9d433a142a92c7b6a2cc46927dba4140da05810b|
|[389-admin-console-1.1.5.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-console-1.1.5.tar.bz2)|admin-console.git|389-admin-console-1.1.5|[AdminConsole](buildingconsole.html#admin-console)|3baf33f3a045fafb6cd7157e448c9b8453f86721|

### 389 Directory Server 1.2.6.1

|Source tarball|git module|git tag|More Info|SHA1SUM|
|--------------|----------|-------|---------|-------|
|[389-ds-base-1.2.6.1.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.2.6.1.tar.bz2)|ds.git|389-ds-base-1.2.6.1|[Building](building.html)|06e84397f93be1fd39bff4eeba981c67d456c6a4|
|[389-admin-1.1.11.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-1.1.11.tar.bz2)|admin.git|389-admin-1.1.11|[AdminServer](../administration/adminserver.html)|31e6ae835161f670a6393f36b269a7ad1fa4e667|
|[389-adminutil-1.1.10.tar.bz2]({{ site.binaries_url }}/binaries/389-adminutil-1.1.10.tar.bz2)|adminutil.git|389-adminutil-1.1.10|[AdminUtil](../administration/adminutil.html)|310be539a4cd31a892858cabf609c0d3acedad92|
|[winsync-1.1.4.tar.bz2]({{ site.binaries_url }}/binaries/winsync-1.1.4.tar.bz2)|winsync.git|winsync-1.1.4|[WindowsSync](../howto/howto-windowssync.html|3e45d315038d0694d7f801bd4911e3f1f524191f|
|[389-console-1.1.6.tar.bz2]({{ site.binaries_url }}/binaries/389-console-1.1.6.tar.bz2)|console.git|389-console-1.1.6|[WindowsSync](../howto/howto-windowsconsole.html|06f7128bc86d1429c6fd0a920ecbb0bac9799206|
|[idm-console-framework-1.1.5.tar.bz2]({{ site.binaries_url }}/binaries/idm-console-framework-1.1.5.tar.bz2)|console(CVS)|FedoraConsoleFramework\_1\_1\_5(CVS)|[buildingconsole.html](buildingconsole.html)|15f1d2af4cac986c6caad39f4ed02191169fcb42|
|[389-ds-console-1.2.3.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-console-1.2.3.tar.bz2)|ds-console.git|389-ds-console-1.2.3|[DirectoryConsole](buildingconsole.html#ds-console)|9d433a142a92c7b6a2cc46927dba4140da05810b|
|[389-admin-console-1.1.5.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-console-1.1.5.tar.bz2)|admin-console.git|389-admin-console-1.1.5|[AdminConsole](buildingconsole.html#admin-console)|3baf33f3a045fafb6cd7157e448c9b8453f86721|

### 389 Directory Server 1.2.5

|Source tarball|git module|git tag|More Info|SHA1SUM|
|--------------|----------|-------|---------|-------|
|[389-ds-base-1.2.5.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.2.5.tar.bz2)|ds.git|389-ds-base-1.2.5|[Building](building.html)|40340cdf1d1816c5a6b97acfb770c1f5ad6f7f4a|
|[389-admin-1.1.10.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-1.1.10.tar.bz2)|admin.git|389-admin-1.1.10|[AdminServer](../administration/adminserver.html)|a1e4f053c6915a500d411306614a6b58c941f93c|
|[389-adminutil-1.1.9.tar.bz2]({{ site.binaries_url }}/binaries/389-adminutil-1.1.9.tar.bz2)|adminutil.git|389-adminutil-1.1.9|[AdminUtil](../administration/adminutil.html)|516cd69f7a0b34f52563a4a5b8e4a6f9b0839177|
|[389-dsgw-1.1.5.tar.bz2]({{ site.binaries_url }}/binaries/389-dsgw-1.1.5.tar.bz2)|dsgw.git|389-dsgw-1.1.5|[DSGW\_Building](../administration/dsgw-building.html)|9ef4a18ddd09a566402f1fd68bef8f774857d680|

### 389 Directory Server 1.2.4

|Source tarball|git module|git tag|More Info|SHA1SUM|
|--------------|----------|-------|---------|-------|
|[389-ds-base-1.2.4.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.2.4.tar.bz2)|ds.git|389-ds-base-1.2.4|[Building](building.html)|54a9257a3b979c5c953e69a45739912f919ebdda|
|[winsync-1.1.3.tar.bz2]({{ site.binaries_url }}/binaries/winsync-1.1.3.tar.bz2)|winsync.git|winsync-1.1.3|[WindowsSync](../howto/howto-windowssync.html|d4b7ee3e75e8fec26bd0a3ebf0f4389d14376529|
|[389-console-1.1.4.a1.tar.bz2]({{ site.binaries_url }}/binaries/389-console-1.1.4.a1.tar.bz2)|console.git|389-console-1.1.4.a1|[WindowsSync](../howto/howto-windowsconsole.html|8fc8616889ef8ef9145fb0198ee02dd5b4b0bcd6|

### 389 Directory Server 1.2.3

Modules are git modules and tags are git tags, except where noted as CVS.

|Source tarball|git module|git tag|More Info|SHA1SUM|
|--------------|----------|-------|---------|-------|
|[389-adminutil-1.1.8.tar.bz2]({{ site.binaries_url }}/binaries/389-adminutil-1.1.8.tar.bz2)|adminutil.git|389-adminutil-1.1.8|[AdminUtil](../administration/adminutil.html)|ff2090c74f63cce65f8222263207ee5442a9e325|
|[389-ds-base-1.2.3.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.2.3.tar.bz2)|ds.git|389-ds-base-1.2.3|[Building](building.html)|f1ed676a3fa2d118c4b57926502bcba9bcd413ef|
|[389-admin-1.1.9.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-1.1.9.tar.bz2)|admin.git,mod\_admserv(CVS),mod\_restartd(CVS)|389-admin-1.1.9,three89Admin\_1\_1\_9(CVS)|[AdminServer](../administration/adminserver.html)|523d0c8b9c88c5c1c1312cc0e89ac15cd07a598c|
|[389-console-1.1.3.tar.bz2]({{ site.binaries_url }}/binaries/389-console-1.1.3.tar.bz2)|console.git|389-console-1.1.3|[389 Console](buildingconsole.html#framework)|b1a5afa6e7039283ac340939d5e1728431370ba9|
|[idm-console-framework-1.1.3.tar.bz2]({{ site.binaries_url }}/binaries/idm-console-framework-1.1.3.tar.bz2)|console(CVS)|FedoraConsoleFramework\_1\_1\_3(CVS)|[buildingconsole.html](buildingconsole.html)|b234a0549e80b739672323e963ae149a5be188df|
|[389-ds-console-1.2.0.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-console-1.2.0.tar.bz2)|ds-console.git|389-ds-console-1.2.0|[DirectoryConsole](buildingconsole.html#ds-console)|403c493f69b94747ea9078799a1f871b71a71d73|
|[389-admin-console-1.1.4.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-console-1.1.4.tar.bz2)|admin-console.git|389-admin-console-1.1.4|[AdmservConsole](buildingconsole.html#admin-console)|29a4ba674b4f532c67ed1303162e5b232bcf9821|
|[389-dsgw-1.1.4.tar.bz2]({{ site.binaries_url }}/binaries/389-dsgw-1.1.4.tar.bz2)|dsgw.git|389-dsgw-1.1.4|[DSGW\_Building](../administration/dsgw-building.html)|52e01146f9b35b46c5deb288806b10624ffff855|
|[winsync-1.1.2.tar.bz2]({{ site.binaries_url }}/binaries/winsync-1.1.2.tar.bz2)|winsync.git|winsync-1.1.2|[WindowsSync](../howto/howto-windowssync.html|7391f4bde7ef8a42bc2722e3f581abe3ac09b639|

### 389 Directory Server 1.2.2

Modules are git modules and tags are git tags, except where noted as CVS.

|Source tarball|git module|git tag|More Info|SHA1SUM|
|--------------|----------|-------|---------|-------|
|[389-adminutil-1.1.8.tar.bz2]({{ site.binaries_url }}/binaries/389-adminutil-1.1.8.tar.bz2)|adminutil.git|389-adminutil-1.1.8|[AdminUtil](../administration/adminutil.html)|ff2090c74f63cce65f8222263207ee5442a9e325|
|[389-ds-base-1.2.2.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-base-1.2.2.tar.bz2)|ds.git|389-ds-base-1.2.2|[Building](building.html)|459aa7228b7ef775db5ba588a6b795db997da4f4|
|[389-admin-1.1.8.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-1.1.8.tar.bz2)|admin.git,mod\_admserv(CVS),mod\_restartd(CVS)|389-admin-1.1.8,three89Admin\_1\_1\_8(CVS)|[AdminServer](../administration/adminserver.html)|4d1eb839581b21053f24f9f0908f20fe60a51c37|
|[389-console-1.1.3.tar.bz2]({{ site.binaries_url }}/binaries/389-console-1.1.3.tar.bz2)|console.git|389-console-1.1.3|[389 Console](buildingconsole.html#framework)|b1a5afa6e7039283ac340939d5e1728431370ba9|
|[idm-console-framework-1.1.3.tar.bz2]({{ site.binaries_url }}/binaries/idm-console-framework-1.1.3.tar.bz2)|console(CVS)|FedoraConsoleFramework\_1\_1\_3(CVS)|[buildingconsole.html](buildingconsole.html)|b234a0549e80b739672323e963ae149a5be188df|
|[389-ds-console-1.2.0.tar.bz2]({{ site.binaries_url }}/binaries/389-ds-console-1.2.0.tar.bz2)|ds-console.git|389-ds-console-1.2.0|[DirectoryConsole](buildingconsole.html#ds-console)|403c493f69b94747ea9078799a1f871b71a71d73|
|[389-admin-console-1.1.4.tar.bz2]({{ site.binaries_url }}/binaries/389-admin-console-1.1.4.tar.bz2)|admin-console.git|389-admin-console-1.1.4|[AdmservConsole](buildingconsole.html#admin-console)|29a4ba674b4f532c67ed1303162e5b232bcf9821|
|[389-dsgw-1.1.4.tar.bz2]({{ site.binaries_url }}/binaries/389-dsgw-1.1.4.tar.bz2)|dsgw.git|389-dsgw-1.1.4|[DSGW\_Building](../administration/dsgw-building.html)|52e01146f9b35b46c5deb288806b10624ffff855|
|[winsync-1.1.0.tar.bz2]({{ site.binaries_url }}/binaries/winsync-1.1.0.tar.bz2)|winsync.git|winsync\_1\_1\_0|[WindowsSync](../howto/howto-windowssync.html|bb661761138c0f67fe1e33ea870c826e2fdb78b8|

### Fedora Directory Server 1.2.0

|Source tarball|CVS module|CVS static tag|More Info|SHA1SUM|
|--------------|----------|--------------|---------|-------|
|[adminutil-1.1.8.tar.bz2]({{ site.binaries_url }}/binaries/adminutil-1.1.8.tar.bz2)|adminutil|adminutil\_1\_1\_8|[AdminUtil](../administration/adminutil.html)|8deb2b018f96270ecb41f3625cdf7069357b25e9|
|[fedora-ds-base-1.2.0.tar.bz2]({{ site.binaries_url }}/binaries/fedora-ds-base-1.2.0.tar.bz2)|ldapserver|FedoraDirSvr\_1\_2\_0|[Building](building.html)|bbce7a98ebbdc13e4ca11c57cb5990a5d4b1bb87|
|[fedora-ds-admin-1.1.7.tar.bz2]({{ site.binaries_url }}/binaries/fedora-ds-admin-1.1.7.tar.bz2)|adminserver,mod\_admserv,mod\_restartd|FedoraDirSrvAdmin\_1\_1\_7|[AdminServer](../administration/adminserver.html)|2018efb83de6ab3af1ff386197d621f07f67b66f|
|[fedora-idm-console-1.1.3.tar.bz2]({{ site.binaries_url }}/binaries/fedora-idm-console-1.1.3.tar.bz2)|fedora-idm-console|FedoraIDMConsole\_1\_1\_3|[Fedora IDM Console](buildingconsole.html#framework)|bc9fd58b7f9266eab3cca025a9030e2c76a67829|
|[idm-console-framework-1.1.3.tar.bz2]({{ site.binaries_url }}/binaries/idm-console-framework-1.1.3.tar.bz2)|console|FedoraConsoleFramework\_1\_1\_3|[buildingconsole.html](buildingconsole.html)|b234a0549e80b739672323e963ae149a5be188df|
|[fedora-ds-console-1.2.0.tar.bz2]({{ site.binaries_url }}/binaries/fedora-ds-console-1.2.0.tar.bz2)|directoryconsole|FedoraDirectoryconsole\_1\_2\_0|[DirectoryConsole](buildingconsole.html#ds-console)|81a6a3647b46d7562bc1dab9e390969aa34ceb8d|
|[fedora-ds-admin-console-1.1.3.tar.bz2]({{ site.binaries_url }}/binaries/fedora-ds-admin-console-1.1.3.tar.bz2)|admservconsole|FedoraAdmservconsole\_1\_1\_3|[AdmservConsole](buildingconsole.html#admin-console)|6ddebd0771a1ad30721e5c93d926a35e7909618c|
|[fedora-ds-dsgw-1.1.2.tar.bz2]({{ site.binaries_url }}/binaries/fedora-ds-dsgw-1.1.2.tar.bz2)|dsgw|FedoraDirSvrDSGW\_1\_1\_2|[DSGW\_Building](../administration/dsgw-building.html)|f0e86c79da993fa8d01c7f3d90eef9c39d69c8d8|
|[winsync-1.1.0.tar.bz2]({{ site.binaries_url }}/binaries/winsync-1.1.0.tar.bz2)|winsync|winsync\_1\_1\_0|[WindowsSync](../howto/howto-windowssync.html|bb661761138c0f67fe1e33ea870c826e2fdb78b8|

### Fedora Directory Server 1.1.3

This includes only the fedora-ds-base package. All of the other packages are the same as for 1.1.2

|Source tarball|CVS module|CVS static tag|More Info|MD5SUM|
|--------------|----------|--------------|---------|------|
|[fedora-ds-base-1.1.3.tar.bz2]({{ site.binaries_url }}/binaries/fedora-ds-base-1.1.3.tar.bz2)|ldapserver|FedoraDirSvr\_1\_1\_3|[Building](building.html)|65aeecb66a6977f7f4706569d02ad8ce|

### Fedora Directory Server 1.1.2

|Source tarball|CVS module|CVS static tag|More Info|MD5SUM|
|--------------|----------|--------------|---------|------|
|[adminutil-1.1.7.tar.bz2]({{ site.binaries_url }}/binaries/adminutil-1.1.7.tar.bz2)|adminutil|adminutil\_1\_1\_7|[AdminUtil](../administration/adminutil.html)|e7d03be4651b36d1213b4f5cc15dfc5c|
|[fedora-ds-base-1.1.2.tar.bz2]({{ site.binaries_url }}/binaries/fedora-ds-base-1.1.2.tar.bz2)|ldapserver|FedoraDirSvr\_1\_1\_2|[Building](building.html)|797c93351e8fcca9bac6326e7270355e|
|[fedora-ds-admin-1.1.6.tar.bz2]({{ site.binaries_url }}/binaries/fedora-ds-admin-1.1.6.tar.bz2)|adminserver,mod\_admserv,mod\_restartd|FedoraDirSrvAdmin\_1\_1\_6|[AdminServer](../administration/adminserver.html)|63a2b5f4496d0cb4b067160fc9da5fd8|
|[idm-console-framework-1.1.2.tar.bz2]({{ site.binaries_url }}/binaries/idm-console-framework-1.1.2.tar.bz2)|console|FedoraConsoleFramework\_1\_1\_2|[buildingconsole.html](buildingconsole.html)|f2db919004fcaf5d6adf6db55b4d589f|
|[fedora-ds-console-1.1.2.tar.bz2]({{ site.binaries_url }}/binaries/fedora-ds-console-1.1.2.tar.bz2)|directoryconsole|FedoraDirectoryconsole\_1\_1\_2|[DirectoryConsole](buildingconsole.html#ds-console)|62964d896042c032143d9bac60abd105|
|[fedora-ds-admin-console-1.1.2.tar.bz2]({{ site.binaries_url }}/binaries/fedora-ds-admin-console-1.1.2.tar.bz2)|admservconsole|FedoraAdmservconsole\_1\_1\_2|[AdmservConsole](buildingconsole.html#admin-console)|e40ffc75263637e886fdf62b20e9a628|
|[fedora-ds-dsgw-1.1.1.tar.bz2]({{ site.binaries_url }}/binaries/fedora-ds-dsgw-1.1.1.tar.bz2)|dsgw|FedoraDirSvrDSGW\_1\_1\_1|[DSGW\_Building](../administration/dsgw-building.html)|fd86e38de705e75296100d7fe9025970|

### Fedora Directory Server 1.1.1

|Source tarball|CVS module|CVS static tag|More Info|MD5SUM|
|--------------|----------|--------------|---------|------|
|[fedora-ds-base-1.1.1.tar.bz2]({{ site.binaries_url }}/binaries/fedora-ds-base-1.1.1.tar.bz2)|ldapserver|FedoraDirSvr111|[Building](building.html)|c525e0412ae4b9582adbd01305126975|
|[idm-console-framework-1.1.1.tar.bz2]({{ site.binaries_url }}/binaries/idm-console-framework-1.1.1.tar.bz2)|console|FedoraConsoleFramework112|[buildingconsole.html](buildingconsole.html)|a23291c9aea256f075b69df981fae42a|
|[fedora-idm-console-1.1.1.tar.bz2]({{ site.binaries_url }}/binaries/fedora-idm-console-1.1.1.tar.bz2)|fedora-idm-console|FedoraIDMConsole112|[IDMConsole](buildingconsole.html#framework)|4c2b16080a3c6e477924091c02d721bf|
|[fedora-ds-console-1.1.1.tar.bz2]({{ site.binaries_url }}/binaries/fedora-ds-console-1.1.1.tar.bz2)|directoryconsole|FedoraDirectoryconsole112|[DirectoryConsole](buildingconsole.html#ds-console)|ee0401937a81ce2466292a4f9b14e20a|
|[fedora-admin-console-1.1.1.tar.bz2]({{ site.binaries_url }}/binaries/fedora-admin-console-1.1.1.tar.bz2)|admservconsole|FedoraAdmservconsole112|[AdmservConsole](buildingconsole.html#admin-console)|e0f16a5a426a2c2bceefb5cfb99ea9c7|
|[fedora-ds-admin-1.1.5.tar.bz2]({{ site.binaries_url }}/binaries/fedora-ds-admin-1.1.5.tar.bz2)|adminserver,mod\_admserv,mod\_restartd|FedoraDirSrvAdmin115|[AdminServer](../administration/adminserver.html)|766c2ab5a7659450ac9fb37fac5ddeb5|
|[adminutil-1.1.6.tar.bz2]({{ site.binaries_url }}/binaries/adminutil-1.1.6.tar.bz2)|adminutil|FedoraAdminutil116|[AdminUtil](../administration/adminutil.html)|b01d441f81d3d260ba84e4f0d5311721|
|[mod\_nss-1.0.7.tar.gz]({{ site.binaries_url }}/binaries/mod_nss-1.0.7.tar.gz)|mod\_nss|mod\_nss107|[mod\_nss](../administration/mod-nss.html)|71107cbc702bf07c6c79843aa92a0e09|

### Fedora Directory Server 1.1.0

These are the sources which were used to build the initial 1.1.0 release.

|Source tarball|CVS module|CVS static tag|More Info|MD5SUM|
|--------------|----------|--------------|---------|------|
|[idm-common-framework-1.1.0.tar.bz2]({{ site.binaries_url }}/binaries/idm-common-framework-1.1.0.tar.bz2)|console|FedoraConsoleFramework111|[buildingconsole.html](buildingconsole.html)|a24d54361b12984b07fc01ff8f8af447|
|[fedora-idm-console-1.1.0.tar.bz2]({{ site.binaries_url }}/binaries/fedora-idm-console-1.1.0.tar.bz2)|fedora-idm-console|FedoraIDMConsole111|[IDMConsole](buildingconsole.html#framework)|e76a8212c6eaaaab3333aa076ca5499d|
|[fedora-ds-console-1.1.0.tar.bz2]({{ site.binaries_url }}/binaries/fedora-ds-console-1.1.0.tar.bz2)|directoryconsole|FedoraDirectoryconsole111|[DirectoryConsole](buildingconsole.html#ds-console)|7b69248b8f18484f03e260a144b1265c|
|[fedora-admin-console-1.1.0.tar.bz2]({{ site.binaries_url }}/binaries/fedora-admin-console-1.1.0.tar.bz2)|admservconsole|FedoraAdmservconsole111|[AdmservConsole](buildingconsole.html#admin-console)|32ecb58f33660705edcd8c3606de750d|
|[fedora-ds-base-1.1.0.tar.bz2]({{ site.binaries_url }}/binaries/fedora-ds-base-1.1.0.tar.bz2)|ldapserver|FedoraDirSvr110|[Building](building.html)|a60d1ce51207e61c48b70aa85ae5e5a5|
|[fedora-ds-admin-1.1.1.tar.bz2]({{ site.binaries_url }}/binaries/fedora-ds-admin-1.1.1.tar.bz2)|adminserver,mod\_admserv,mod\_restartd|FedoraDirSrvAdmin112|[AdminServer](../administration/adminserver.html)|f50f2b6c983851c5e912047807bbcca6|
|[adminutil-1.1.5.tar.bz2]({{ site.binaries_url }}/binaries/adminutil-1.1.5.tar.bz2)|adminutil|FedoraAdminutil115|[AdminUtil](../administration/adminutil.html)|1ce95159db07040d7095b805e9b3b533|
|[mod\_nss-1.0.7.tar.gz]({{ site.binaries_url }}/binaries/mod_nss-1.0.7.tar.gz)|mod\_nss|mod\_nss107|[mod\_nss](../administration/mod-nss.html)|71107cbc702bf07c6c79843aa92a0e09|

### 389 Directory Password Synchronization 1.1.6

This is the source which were used to build the 389 Directory Password Synchronization.

|Source tarball|git module|git tag|MD5SUM|
|--------------|----------|-------|------|
|[389-passsync-1.1.6.tar.bz2]({{ site.binaries_url }}/binaries/389-passsync-1.1.6.tar.bz2)|winsync|winsync-1.1.6|13493549a90182e064ce7987f869c56f64e48ac0|


