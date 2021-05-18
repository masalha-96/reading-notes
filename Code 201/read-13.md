# HTML5

The article discusses the history of storing data in web browsers so it can be reused after refreshing the page, closing the browser, or sometimes after restarting the device.

For a long time, cookies were the main way to store information about users visiting your app or website. Then, HTML5 appeared on the scene and introduced LocalStorage as another data storage option.

## Cookies vs. LocalStorage: 

.| Definition | Capacity | Use | Limitation
---|---|---|---|---
Cookies | Small text files that are placed on a user’s computer by a website. | maximum capacity of 4KB. | Cookies are used in different ways, such as in storing the pages visited on a site or a user’s login information. | They are limited in that they can only store strings.
LocalStorage |  it’s a way for web pages to store named key/value pairs locally, within the client web browser. | LocalStorage can hold up to 5MB of information. | not stable internet connection, more protection to the client's privacy, save games data. | storage space is the main limitation 



++
## How to use localStorage in JS: 
### 1. set function 
* I used it, to covert my array to string using JSON.stringify() method,  then to save my data into localStorage, because localStorage contain strings only.

**function set()** 
{

    // save my data into localStorage 
    let mydata = JSON.stringify(myImages);
    localStorage.setItem('dataKey', dataValue);
}

* myImages :: global array that contains all my objects.

<br>
<br>


### 2. get function 
* I used it, to covert my array to numbers again with JSON.parse() method.

**function getStoredItems()** {

{

    let stringData = localStorage.getItem('dataKey');
    let normalData = JSON.parse(stringData);

    if ( normalData !== null ) {
        myImages = normalData;
    }
    
}

