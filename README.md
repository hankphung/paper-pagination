# paper-pagination
Polymer pagination element. Input record count, pagesize to get list of page chooser.
![screenshot-localhost 8080 2016-09-16 08-39-04](https://cloud.githubusercontent.com/assets/2910175/18572865/2a8267ee-7be9-11e6-945c-b651b30e8218.png)

## Setup
Clone this repo or install by bower. `bower install paper-pagination`
## Usage
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
