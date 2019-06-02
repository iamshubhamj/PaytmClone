# PaytmClone
Note : For admin login and store updated wallet txn used diffrent schema.

Done this Sample in Node js Version v10.15.3 in loopback Framework.
dowload this clone
setup of loopback
#Run npm install request
#Run nodemon .
#server will start on 3000 port

Please find below few API's URL and  request.

registration

............................

https://localhost:3000/api/user/signup

{
	"phoneNumber" : "6393379964",
	"password"    : "Develop@123",
	"emailId"     : "shubhamjaiswal00@gmail.com"
}

otp Validation

..............................

https://localhost:3000/api/user/otp_Validation

{
	"otp" : "551951"
}


Login

................................

https://localhost:3000/api/user/login

{
	"phoneNumber" : "6393379964",
	"password"    : "Develop@123"
}

AddMoney
..................................

https://localhost:3000/api/user/add_Money

{
	"phoneNumber" : "6393379964",
   "addBalance": "200"
}

Transfer Money
..............................
https://localhost:3000/api/userTxn/transfer_Amount

{
	 "payerNumber": "6393379964",
     "payeeNumber": "8800791689",
     "amount"     : "150"
}

Txn History
.................

https://localhost:3000/api/userTxn/txnHistory

{
	 "payeeNumber": "6393379964"
    
}

Admin WalletView
..................................

https://localhost:3000/api/admin/loadWallet
{
  "phoneNumber": phoneNumber,
  "walletBalance": walletBalance
}
allTxn
.............................

{
	"user"        : "admin",
	"password"    : "admin@123"
}
