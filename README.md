
# PUBG-AWS-API-Gateway-Proxy
Proxy for use with the PUBG AWS API Gateway Proxy

## Setup
1. Go to https://developer.pubg.com/apps?locale=en and register for an API key
2. Replace all instances of `<<YOUR_PUBG_API_KEY>>` in the `pubg.json` with your API key
3. Create an aws account https://aws.amazon.com/account/ (you can use the free tier)
4. Go to API Gateway and create a new API
5. Set the API up with the following:
  * Specify a `REST` API
  * Select `Import from Swagger or Open API 3` from the 
  * Select `pubg.json` as the Swagger File
6. Hit create
7. Go to resources and in the actions menu hit deploy
8. Go to stages to find your proxy URL
9. Test with the provided POSTMAN collection, here's the collection variables:
```
pubg_aws_proxy:AWS_API_GATEWAY_URL
pubg_account:account.1c479e79987041cfa3269a3e7544ed35
pubg_player:Stevethemage
pubg_match:e0116b91-65e0-4ded-8e59-2f675ca03902
pubg_tournament:cn-ppe
pubg_season:division.bro.official.2017-beta
pubg_aws_platform:steam
```
10. Enjoy!
