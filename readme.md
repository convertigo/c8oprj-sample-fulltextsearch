


# demo_full_text_search

### Full Text Search

## Demo back-end project for Studio No Code.

In the resources folder you will find:
 - export - Radios.csv => Data to import in your Baserow workspace.
 - Full TEXT SEARCH 2.c8oforms => Application to import from the Studio No Code Dashboard.
 
 [Convertigo No Code Studio](https://www.convertigo.com/fr/platform/no-code-studio)


For more technical informations : [documentation](./project.md)

- [Installation](#installation)
- [Sequences](#sequences)
    - [formssource_RADIOS](#formssource_radios)
    - [formssource_RADIOS_FTS](#formssource_radios_fts)
    - [RADIOSRadiosFTSList](#radiosradiosftslist)
    - [RADIOSRadiosGridList](#radiosradiosgridlist)


## Installation

1. In your Convertigo Studio click on ![](https://github.com/convertigo/convertigo/blob/develop/eclipse-plugin-studio/icons/studio/project_import.gif?raw=true "Import a project in treeview") to import a project in the treeview
2. In the import wizard

   ![](https://github.com/convertigo/convertigo/blob/develop/eclipse-plugin-studio/tomcat/webapps/convertigo/templates/ftl/project_import_wzd.png?raw=true "Import Project")
   
   paste the text below into the `Project remote URL` field:
   <table>
     <tr><td>Usage</td><td>Click the copy button at the end of the line</td></tr>
     <tr><td>To contribute</td><td>

     ```
     demo_full_text_search=https://github.com/convertigo/c8oprj-sample-fulltextsearch.git:branch=master
     ```
     </td></tr>
     <tr><td>To simply use</td><td>

     ```
     demo_full_text_search=https://github.com/convertigo/c8oprj-sample-fulltextsearch/archive/master.zip
     ```
     </td></tr>
    </table>
3. Click the `Finish` button. This will automatically import the __demo_full_text_search__ project


## Sequences

### formssource_RADIOS

Can be filtered out providing the 'filter' variable

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>forms_filtre</td><td>Perform a full text search</td>
</tr>
</table>

### formssource_RADIOS_FTS

Performs a full text search on every columns for every terms entered

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>forms_filtre</td><td>Perform a full text search</td>
</tr>
</table>

### RADIOSRadiosFTSList

## List rows of Radios from RADIOS

Uses the 'searched_string' variable to perform a complex search of every term of the string in each table columns.

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>page</td><td>Defines which page of rows should be returned.</td>
</tr>
<tr>
<td>searched_string</td><td>Strings to search in every Baserow table columns</td>
</tr>
<tr>
<td>size</td><td>Defines how many rows should be returned per page.</td>
</tr>
</table>

### RADIOSRadiosGridList

## List rows of Radios from RADIOS

Uses the 'search' variable to perform a basic text search in each columns.

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>page</td><td>Defines which page of rows should be returned.</td>
</tr>
<tr>
<td>search</td><td>If provided only rows with data that matches the search query are going to be returned.</td>
</tr>
<tr>
<td>size</td><td>Defines how many rows should be returned per page.</td>
</tr>
</table>



