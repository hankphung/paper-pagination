# paper-pagination
Polymer pagination element. Input record count, pagesize to get list of page chooser.

## Setup
clone this repo or install by bower.
## Usage
```
  <paper-pagin page-size="5" total="21" current-page="{{current}}" offset="{{ose}}"></paper-pagin>
  <span> page:{{current}} <br/> offset:{{ose}}</span>
```
To observe the change on current, use observer
```javascript
  observer:['_currentPageChange(current)'],
  _currentPageChange:function(c){
    console.log(c)
  },
```
