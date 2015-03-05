#Silverstripe MetaExtension (Title & Keywords)#

Re-adds 'MetaTitle' and 'MetaKeywords' fields that were removed in SilverStripe 3.1.

###Download:###

Simply clone or download this repository, copy it into your SilverStripe installation folder, then run `dev/build`.

###Usage:###

In Page Head e.g.:

```
<title><% if $MetaTitle %>$MetaTitle<% else %>$Title<% end_if %> &raquo; $SiteConfig.Title</title>
```

and

```
<% if $MetaKeywords %><meta name="keywords" content="$MetaKeywords"/><% end_if %>
```
