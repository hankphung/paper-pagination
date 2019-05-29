```

   /\˜˜/   /\˜˜/\   
  /__\/   /__\/__\    
 /\  /   /\  /\  /\ 
/__\/   /__\/  \/__\  Polymer
\  /\  /\  /   /\  /
 \/__\/__\/   /__\/   
  \  /\  /   /\  /  
   \/__\/   /__\/   

```
# paper-pagination
Polymer pagination element. Input record count, pagesize to get list of page chooser. [Demo](https://hankphung.github.io/paper-pagination/components/paper-pagination/demo/)
![screenshot-localhost 8080 2016-09-16 08-39-04](https://cloud.githubusercontent.com/assets/2910175/18572865/2a8267ee-7be9-11e6-945c-b651b30e8218.png)

## Setup
Clone this repo or install by bower. `bower install paper-pagination`
## Document
**Properties**

Properties | Type| Description
------------ | ------------- | -------------
pageSize | Number | Number of items per page
total | Number | Total items count
rangeSize | Number | Number of visible page item on large collection.
currentPage | Number | Current selected page
hidden | Number | hidden if pageSize == 1
hiddenFirstPageButton | Boolean (*readonly*)
hiddenLastPageButton | Boolean (*readonly*)
hiddenNextPageButton | Boolean (*readonly*)
hiddenPreviousPageButton | Boolean (*readonly*)
## Sample
```
  <paper-pagination page-size="5" total="21" current-page="{{currentPage}}"></paper-pagination>
  <span> page:{{currentPage}></span>
```
To observe the change on currentPage, use observer
```javascript
  observer:['_currentPageChange(currentPage)'],
  _currentPageChange:function(c){
    console.log(c)
  },
```
