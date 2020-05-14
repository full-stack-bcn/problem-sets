
Redux
=====

Reducers
--------

1. Let's do a web application which can do search queries. The class ``SearchState``
   defines a type of object which can hold the state of this app, with some fields
   and some methods:
   ```js
   class SearchState {
     constructor() {
       this.query = "";
       this.loading = false;
       this.results = [];
     }

     setQuery(query) {
       this.query = query;
     }
     beginLoading() {
       this.loading = false;
     }
     setResults(results) {
       this.loading = false;
       this.results = results;
     }
   }
   ```
   Implement a Redux reducer that mirrors the functionality in this class.