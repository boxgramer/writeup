
# Note : 2025-02-27 Portswigger lab

### Metodelogy
 1. Investigate the system to retrieve a list of features
 2. Discribe the feature and explain how it works
 3. List possible vulnerabilities and group by feature
 4. Proof of concept for possible vulnerabilities
 5. What is the impact of the vulnerabilities after the proof of concept ? 


# ==========================================================================================================

>  website e-commerse with check stock and  auth 


## feature:      
### check stock
1. using fetch method javascrit to request the server
2. POST /product/stock using parameter  ``` stockApi=http%3A%2F%2Fstock.weliketoshop.net%3A8080%2Fproduct%2Fstock%2Fcheck%3FproductId%3D1%26storeId%3D1 ``` decode to ``` http://stock.weliketoshop.net:8080/product/stock/check?productId=1&storeId=1 ```  and got response  

``` 
HTTP/1.1 200 OK
Content-Type: text/plain; charset=utf-8
Content-Encoding: gzip
Connection: close
X-Frame-Options: SAMEORIGIN
Content-Length: 3

971 
```
3. 


## vulnerabilities : 
1. ssrf( server side request forgery)
## Proof of concept:
## impact

# =====================================================================================================================================================================
