# Javascript

### 28-11-2023

<table>
<tr>
<th>My code</th>
<th>Improved Code</th>
</tr>
  <tr>
  <td>
    
```js
// Count the occurrences of each status

const countStatus = {};
uniqueStatuses.forEach(uniqueItem => {
  allStatuses.forEach(item => {
    if (uniqueItem === item) {
      countStatus[uniqueItem] = (countStatus[uniqueItem] || 0) + 1;
    }
  })
})

// // added all components  new property in the object
let sum = 0;
uniqueStatuses['all component'] = Object.values(tabsStatus).reduce((acc, item) => {
  sum += item;
  return acc + item;
}, 0);
```

  </td>
  <td>

```js
// Count the occurrences of each status improved version
const tabsStatus = allStatuses.reduce((acc, status) => {
  acc[status] = (acc[status] || 0) + 1;
  acc['all component'] = (acc['all component'] || 0) + 1;
  return acc;
}, {});
```

</td>
</tr>
</table>

<table>
  <tr>
    <td>
    
  ```jsx
  
  ```  
    
  </td>
  <td></td>
  </tr>
</table>
