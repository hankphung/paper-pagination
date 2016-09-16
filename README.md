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
Polymer pagination element. Input record count, pagesize to get list of page chooser.
![screenshot-localhost 8080 2016-09-16 08-39-04](https://cloud.githubusercontent.com/assets/2910175/18572865/2a8267ee-7be9-11e6-945c-b651b30e8218.png)

## Setup
Clone this repo or install by bower. `bower install paper-pagination`
## Document
**Properties**
|pageSize|Number| Number of items per page|
|total|Number| Total items count|
|rangeSize| Number| Number of visible page item on large collection.|
|currentPage|Number(*readonly*)| Current selected page|
|offset|Number(*readonly*)| Use for offset (sql) or skip(blueprint API)|
## Sample
```
  <paper-pagin page-size="5" total="21" current-page="{{current}}" offset="{{skip}}"></paper-pagin>
  <span> page:{{current}} <br/> offset:{{skip}}</span>
```
To observe the change on current, use observer
```javascript
  observer:['_currentPageChange(current)'],
  _currentPageChange:function(c){
    console.log(c)
  },
```
