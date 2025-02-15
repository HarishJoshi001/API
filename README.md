Calculation that can be done here

1. Addition
2. Subtraction


**1. REST**

***For addition***

GET ```http://localhost:8080/api/add?num1=2&num2=3```

![image](https://github.com/user-attachments/assets/e8a65cb5-ea96-4771-8fc5-5f05992ed42f)


***For subtraction***

GET ```http://localhost:8080/api/subtract?num1=20&num2=3.3```

![image](https://github.com/user-attachments/assets/4046b7d9-142e-4778-88de-46f785ee71bf)




**2. SOAP**

For both addition and subtraction, use

POST ```http://localhost:8080/ws```

***For addition***


```  
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
                  xmlns:web="http://harish.com/calculator">
   <soapenv:Header/>
   <soapenv:Body>
      <web:AddRequest>
         <web:number1>10.5</web:number1>
         <web:number2>5.5</web:number2>
      </web:AddRequest>
   </soapenv:Body>
</soapenv:Envelope>
```

![image](https://github.com/user-attachments/assets/2018fbdb-bcfc-4e66-ab9e-b082e0fb91ce)

***For subtraction***
```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
                  xmlns:web="http://harish.com/calculator">
   <soapenv:Header/>
   <soapenv:Body>
      <web:SubtractRequest>
         <web:number1>10.5</web:number1>
         <web:number2>5.5</web:number2>
      </web:SubtractRequest>
   </soapenv:Body>
</soapenv:Envelope>
```
![image](https://github.com/user-attachments/assets/26366761-7e51-4a05-98a6-6bd67338672d)
