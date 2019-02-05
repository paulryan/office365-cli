# spo sitedesign run list

Lists information about site designs applied to the specified site

## Usage

```sh
spo sitedesign run list [options]
```

## Options

Option|Description
------|-----------
`--help`|output usage information
`-u, --webUrl <webUrl>`|The URL of the site for which to list applied site designs
`-i, --siteDesignId [siteDesignId]`|The ID of the site design for which to display information
`-o, --output [output]`|Output type. `json|text`. Default `text`
`--verbose`|Runs command with verbose logging
`--debug`|Runs command with debug logging

!!! important
    Before using this command, log in to a SharePoint Online site, using the [spo login](../login.md) command.

## Remarks

To list information about site designs applied to the specified site, you have to first log in to a SharePoint site using the [spo login](../login.md) command, eg. `spo login https://contoso.sharepoint.com`.

## Examples

List site designs applied to the specified site

```sh
spo sitedesign run list --webUrl https://contoso.sharepoint.com/sites/team-a
```

List information about the specified site design applied to the specified site

```sh
spo sitedesign run list --webUrl https://contoso.sharepoint.com/sites/team-a --siteDesignId 6ec3ca5b-d04b-4381-b169-61378556d76e
```

## More information

- SharePoint site design and site script overview: [https://docs.microsoft.com/en-us/sharepoint/dev/declarative-customization/site-design-overview](https://docs.microsoft.com/en-us/sharepoint/dev/declarative-customization/site-design-overview)