---
title: Embedding XERO Viewer in the EMR system
last_updated: 'Sep 18, 2017'
keywords: 'tags, navigation, buttons, links, association'
summary: null
sidebar: mydoc_sidebar
toc: false
permalink: embedding-xero-viewer-in-emr.html
folder: api
published: false
---


{% include callout.html content="Consult your EMR documentation for information about how to embed a URL into your client. If you require HTML markup for the integration, you can use an iFrame. For information about iFrames, see [http://www.w3.org/TR/html4/present/frames.html#h-16.5](http://www.w3.org/TR/html4/present/frames.html#h-16.5)." type="success" %} 




## Using HTML iFrames
The HTML iFrame element enables you to embed the XERO Viewer application within a web-based EMR system. iFrames are supported in all major browsers, including Internet Explorer and Mozilla Firefox. The two documents remain independent of one another, but the user sees them as an integrated web page. When you embed XERO Viewer into the user interface of the EMR, the user does not have additional windows to manage. Content from the EMR (such as a radiology report or clinical information) is displayed alongside the images. This is a test entry in prose.io.

The following example shows a basic iFrame element and its contents:

```html
<iframe src="
insert_URL_here" attributes>
Alternate content for web browsers that do not support iframes. 
</iframe>
```

The following iFrame element embeds XERO Viewer into an existing web page.

```html
The EMR integrated with XERO Viewer.
<iframe id="frame" name="frame" 
src="http://host_name/?theme=lightEpr&PatientID=27" 
class="frames" width="70%" height="350" frameborder="0"></iframe>
```

To embed a different web page, change the URL to which the SRC element points. For example, to embed the Google website into a web page, the same code looks like this:

```html
The EMR integrated with Google.
<iframe id="frame" name="frame" src="http://www.google.com" 
class="frames" width="70%" height="350" frameborder="0"></iframe>
```

## iFrame standard attributes

<table>
<colgroup>
<col width="15%" />
<col width="45%" />
<col width="15%" />
<col width="15%" />
</colgroup>
<thead>
<tr class="header">
<th>Attribute</th>
<th>Description</th>
<th>Values</th>
<th>Requirement</th>
</tr>
</thead>
<tbody>
<tr>
<td markdown="span">class</td>
<td markdown="span">Specifies a classname for an element</td>
<td markdown="span"><i>classname</i></td>
<td markdown="span">Optional</td>
</tr>
<tr>
<td markdown="span">id</td>
<td markdown="span">Specifies a unique ID for an element</td>
<td markdown="span"><i>id</i></td>
<td markdown="span">Optional</td>
</tr>
<tr>
<td markdown="span">style</td>
<td markdown="span">Specifies an inline style for an element</td>
<td markdown="span"><i>style_definition</i></td>
<td markdown="span">Optional</td>
</tr>
<tr>
<td markdown="span">title</td>
<td markdown="span">Specifies extra information about an element</td>
<td markdown="span"><i>text</i></td>
<td markdown="span">Optional</td>
</tr>
</tbody>
</table>

{% include links.html %}
