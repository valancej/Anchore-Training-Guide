## Whitelists

A whitelist contains one or more exceptions that can be used during policy evaluation. For example allowing a CVE to be excluded from policy evaluation.

The Whitelists tab shows a list of whitelists present in the policy bundle. Whitelists are an optional element of the bundle and a policy bundle may contain multiple whitelists.

![alt text](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/36005886174/original/QcIMlYGZ38WVgXZsWs4IIUOCsJB9hXkYvA?1525313680)

### Adding a New Whitelist

![alt text](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/36005886181/original/4rW65Xi4nbuhL235nfl3idv6c9kEFdqsfQ.png?1525313704) The Add New Whitelist button launches a dialog to create a new, empty whitelist.

The Whitelist name is required and should be unique. 

The description is optional but recommended. Often the description is updated as new entries are added to the whitelist to explain any background.
For example "Updated to account for false positive in glibc library"

![alt text](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/36005968241/original/kFEH1SoOJD1mwyVlgWZdwksE_WNmzNdR6w?1525383531)

### Uploading a Whitelist 

![alt text](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/36005968389/original/w99jICp3DrpvO9WeS0HBRU1_7E1GNdD92w?1525383679) If you have a JSON document containing an existing whitelist then this may be uploaded into the Anchore Engine.

Selecting the Upload whitelist button will present a dialog allowing for a whitelist file to be uploaded or manually edited in the native JSON format.

![alt text](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/36005886199/original/8hjW9RcMpLlQGGAwx6WqyWdIWbCPQq4DlA.png?1525313728)

Whitelist files can be dragged into the dropzone, indicated by a blue plus sign, or clicking in the dropzone will open a file selector dialog allowing a file to be loaded from the local filesystem.

Selecting OK will perform validation on the whitelist. Only validated whitelists may be stored by the Anchore Engine.

### Copying a Whitelist

An existing whitelist can be copied using the Tools drop down and selecting the Copy Whitelist option.

A new dialog will be presented in which a unique name for the Whitelist should be entered.

The description is optional but recommended. Often the description is updated as new entries are added to the whitelist to explain any background.

![alt text](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/36006092975/original/0OuMd-rA0QNO4JRGYuXlqoUfRND9ppU7Lw?1525622682)

### Downloading Whitelists

An existing whitelist can be downloaded as a JSON file by using the Tools drop down menu and selecting Download to JSON

### Editing Whitelists

The Whitelist editor allows new whitelist entries to be created and existing entries to be edited or removed.

The Anchore Engine supports whitelisting any policy trigger however the whitelist editor currently supports only adding Anchore Security checks, allowing vulnerabilities to be whitelisted.

A vulnerabilities whitelist entry includes two elements:

![alt text](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/36006092383/original/pxrKWhMCTRM3U3i4h75c9mJxBlgPQSewIg?1525620892)

The CVE/Vulnerability field contains the vulnerability that should be matched by the whitelist. This can include wildcards.

For example: CVE-2017-7246. This format should match the format of the CVEs shown in the image vulnerabilities report.
Wildcards are supported however car should be taken with using wildcards to prevent whitelisting too many vulnerabilities.

![alt text](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/36006092394/original/w7vE01yxTKMVAgImhg4VAeWUS5UcgGOxqw?1525620914)

The package name field contains the package that should be matched with a vulnerability.
For example libc-bin.

Wildcards are also supported within the Package name field.

A whitelist entry may include entries for both the CVE and Package field to specify an exact match, for example: Vulnerability: CVE-2005-2541  Package: tar

In other cases wildcards may be used where a multiple packages may match a vulnerability. For example in a situation where multiple packages are built from the same source.  Vulnerability: CVE-2017-9000  Package: bind-*

In this example the packages bind-utils, bind-libs and bind-license will all be whitelisted for CVE-2017-9000



Special care should be taken with wildcards in the CVE / Vulnerability Identifier field. In most cases a specific vulnerability identifier will be entered. In some exceptional cases a wild card in this field may be appropriate.

A good example of a valid use case for a wildcard in the CVE / Vulnerability Identifier field is the bind-license package. This package include a single copyright text file and is included by default in all CentOS:7 images. CVEs that are reported against the Bind project are typically applied to all packages built from the Bind source package. So when a CVE is found in Bind it is common to see a CVE reported against the bind-license package. To address this use case it is useful to add a whitelist entry for any vulnerability (*) to the bind-license package.



Whitelist entries can be edited be pressing the ![alt text](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/36006092875/original/ok6sCHZxlOnuHPchG42gjvySLV0EnnKQcw?1525622326) button and can be removed using the Remove button.

Ensure that all changes are saved before exiting out of the Edit Whitelist Items Page. At that point the edits will be sent to the Anchore Engine.

![alt text](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/36006092809/original/6M9u8mXr1Ue_aehYuSkEuA4wmUSJcbvFmA?1525622139)

![alt text](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/36005886174/original/QcIMlYGZ38WVgXZsWs4IIUOCsJB9hXkYvA?1525313680)




