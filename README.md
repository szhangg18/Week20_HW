# Week20_HW
## Associate Profit Splitter
First, deploy the contract with the 3 addresses in the constructor
![image](https://user-images.githubusercontent.com/86904683/149614478-103c5893-e4d6-4b3f-ba1a-8896cfc1dbfd.png)

Any Ether deposited using the deposit function will automatically be split equally between these addresses. Any Ether sent to the contract address will automatically trigger the deposit function. 

## Tiered Profit Splitter
First, deploy the contract with the 3 addresses in the constructor
![image](https://user-images.githubusercontent.com/86904683/149614454-85d67885-a638-4982-be28-fda50bc2d96c.png)

Once deployed, you can edit the transaction value at the top then press "deposit", this will automatically deposit that amount of Ether from your currently connected web3 addresses, and allocate it to the 3 addresses provided in the contructor. For example, this is the result after 1 Ether was deposited. 
![image](https://user-images.githubusercontent.com/86904683/149614443-cc5be3bf-b487-43a9-8e26-17a6542575aa.png)

Any Ether sent to the contract address will automatically trigger the deposit function. 

## Deferred Equity Plan
First, deploy the contract with the address of the employee 
![image](https://user-images.githubusercontent.com/86904683/149614516-5a89945b-5392-44f9-a991-2a9ddf6f3a05.png)

By default, this will allocate 1000 shares to the employee, vested over 4 years with a linear unlock rate each year. However, this can be updated by changing the `total_shares`, `annual_distribution` and `interval`. Please ensure the total shares is exactly divisible by the annual distribution. 

![image](https://user-images.githubusercontent.com/86904683/149614609-92453e16-5793-4cf2-b6d3-186f127a7f67.png)

Once the contract is set up, the employee's address may use the `distribute` function, and if there are any available shares to be claimed it will execute. You may also run the `shares_distributed` function to see the total amount claimed, in this example there are 750 shares claimed. 
![image](https://user-images.githubusercontent.com/86904683/149614652-5c2ec5f1-ae89-4daf-b42e-d40ed3ab6367.png)
