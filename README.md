

# dotcms-AdvancedXMLSitemapJob
A Powered version of dotCMS' XMLSitemapJob 

## Author: Giacomo Petillo @DjacomoIT


### Configuration:

```
org.dotcms.plugins.XMLSitemap.USE_PERMALINKS=true to org.dotcms.plugins.XMLSitemap.USE_PERMALINKS=false
org.dotcms.plugins.XMLSitemap.USE_STRUCTURE_URL_MAP=true or org.dotcms.plugins.XMLSitemap.USE_STRUCTURE_URL_MAP=false
```


### Usage:

This plugin generates a sitemap index file for each host with the following path:
```
http://server.name.com/sitemap_index.xml
http://server1.name.com/sitemap_index.xml
http://server2.name.com/sitemap_index.xml
http://server3.name.com/sitemap_index.xml
```
Each sitemap index file will have a link to every sitemap file on your host. The plugin will create one sitemap file for every 50,000 entries. (50,000 URLs and must be no larger than 9MB (10,485,760))
and will compress it and add it to your sitemap index. Each file will be saved on your host under the folder: /XMLSitemaps/ with the name: xmlSitemapGenerated<N>.xml.gz.

Each sitemap file has a list of all the pages, folders, files and menu links that are noted as Show on Menu in dotCMS. It also adds one permalink entry for each piece of
content for each structure that has a detail page defined on your host.
 

### More Info:

If you need more info about sitemaps protocol you could check this page http://www.sitemaps.org/protocol.php



