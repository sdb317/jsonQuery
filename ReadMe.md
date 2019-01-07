# Visually query JSON data using `jsonpath` syntax

A simple tool to use an XPath-like syntax to query JSON data structures

1. Enter the [jsonpath](https://goessner.net/articles/JsonPath/) query
2. Paste the JSON source on the left (it will be automatically formatted)
3. See the JSON results on the right

The query is automatically re-run whenever the query or the source changes.

Instructions: Browse `jsonQuery.html` or, if you are on Windows, run `mshta <FullPath>jsonQuery.hta` from the command line for a stand-alone instance.


Example: Once your query to return all 'name' objects works, you can embed it in your Javascript code as follows:

```
<script type='text/javascript' src='jsonpath-0.8.0.js'></script>
<script type='text/javascript'>

    var jsonSource = JSON.parse('{"people": [{"name":  "Simon"}]}');
    var jsonResults = jsonPath(jsonSource, '$..name', 'VALUE');

</script>
```


Credits to:

* [Stefan Goessner](https://goessner.net/articles/JsonPath/)
* [jQuery](https://jquery.com/)
* [Ace Editor](https://ace.c9.io/)
* [jsonpath.com](http://jsonpath.com/)

