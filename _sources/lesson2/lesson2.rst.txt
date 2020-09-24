Lesson2 --> Setup AWS Access Key & Secret Key
==============================================

- Setup the Key ID and Secret Key for AWS

1. Click on "Cloud Accounts" tab on the UDF Blue print

2. Copy the API Key & API Secret key 

3. Go to the ubuntu UDF Shell and configure the following

```    aws configure``` 

```    AWS Access Key ID [****************CGGT]:XXXXXXXXXXXXX```

```    AWS Secret Access Key [****************QmTY]:XXXXXXXXXXX``` 



4. Go to Blue Print on the UDF and click on Console URL link use the Console PAssword and username as udf

5. Change directory to ```cd consul-tg-env``` and execute ```make all```

.. image:: /_static/makefail.png

6. Login to AWS Console by going to UDF Blueprint --> Cloud Accounts --> Console URL

7. Use the https link above ```OptInRequired: In order to use this AWS Marketplace product you Error```

8. Click on https://console.aws.amazon.com/marketplace/home?region=us-west-2#/subscriptions/U1VCU0NSSVBUSU9OQEBAOTI5Y2EwZDgtYzJkNy00MDY4LThmOWEtZWI3NWE2NzdhZmVk

                      or

 search for F5 BIG-IP Virtual Edition - BEST (PAYG, 1Gbps)

9. Sunsbcribe to the trial service and Accept all terms.

.. note:: Give like 2 mintutes and make sure you have subscribed to the F5 BIG-IP

