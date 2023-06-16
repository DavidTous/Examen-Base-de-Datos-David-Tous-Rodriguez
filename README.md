# Examen-Base-de-Datos-David-Tous-Rodriguez
1 

Select * 
From Customers 

2 

SELECT MAX(customerid),MAX(customerName),MAX(contactName), MAX(Address) , Max(city),Max(PostalCode),Max(country)  
FROM Customers; 

3 

Select CustomerName,City 
From customers; 

4 

Select Disctint Country 
From Customers 

5 

Select* 
From customers 
Where Country = ‘Mexico’; 

6 

Select* 
From customers 
Where Country = ‘Germany’ AND City=’Berlin’; 
7 

Select products.productName,Categories.CategoryName  
From Products  
Inner Join Categories  
ON Products.CategoryID= Categories.CategoryID; 

8 

Select products.productName,Categories.CategoryName   
From Products   
Inner Join Categories   
ON Products.CategoryID= Categories.CategoryID 
Inner Join Suppliers  
ON products.SupplierID = suppliers.SupplierID; 

9 

Select count(productID)  
From products 
Inner Join Categories  
ON Products.CategoryID= Categories.CategoryID  
Group By categories.CategoryName; 

10 

Select count(productID)  
From products 
Inner Join Categories  
ON Products.CategoryID= Categories.CategoryID  
Where Products.ProductName LIKE ‘P%’ 
Group By categories.CategoryName; 


