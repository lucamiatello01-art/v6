Broker_Agent_V6_Enhanced.const API_KEY = "LA_TUA_API_KEY";

async function getApplePrice() {

  const response = await fetch(
    `https://api.twelvedata.com/quote?symbol=AAPL&apikey=${API_KEY}`
  );

  const data = await response.json();

  console.log(data);

}html
getApplePrice();
