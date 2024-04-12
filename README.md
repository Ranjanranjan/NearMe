# Ex04 Places Around Me
#Date: 12-04-24
## AIM
To develop a website to display details about the places around my house.

## DESIGN STEPS

### STEP 1
Create a Django admin interface.

### STEP 2
Download your city map from Google.

### STEP 3
Using ```<map>``` tag name the map.

### STEP 4
Create clickable regions in the image using ```<area>``` tag.

### STEP 5
Write HTML programs for all the regions identified.

### STEP 6
Execute the programs and publish them.

## CODE
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ImageMap</title>
</head>
<style>
    *{margin: 0;}
</style>
<script>
    function coordinate(event)
    {
        let x = event.clientX;
        let y = event.clientY;
        document.getElementById("Text1").value=x;
        document.getElementById("Text2").value=y;
    }
</script>
<body>
    <IMG src="bg.png" width="1535" height="650" usemap="#MapNew" onmousemove="coordinate(event)">
        <MAP name="MapNew">
            <AREA shape="rect" coords="160,359,376,443" href="https://www.makemytrip.com/hotels/hotel-listing/?topHtlId=201712071752368734&city=CTMAA&country=IN&checkin=04132024&checkout=04142024&roomStayQualifier=2e0e&totalGuestCount=2&roomCount=1&cmp=googlehoteldfinder_DH_META_Paid_selected_IN_mapresults_201712071752368734&_uCurrency=INR&Campaign=20613919640&locusId=CTMAA&locusType=city&mtkeys=b1e79af8-c554-48b3-a52c-85fea70907c2&au=&gclid=Cj0KCQjwlN6wBhCcARIsAKZvD5iBWH_sKzcQ-sYrPVV0CsKUtGbCrrPjzCzd6cFU2R0VyBaiO8_RWIQaAlTaEALw_wcB" title="Moon view beach resort">
                <AREA shape="rect" coords="406,278,536,332" href="https://www.agoda.com/search?campaignid=21176660567&searchdatetype=selected&lt=1&numberofchildren=0&childages=&gsite=mapresults&partnercurrency=INR&roomid=655899473&pricetax=330.62&pricetotal=3085.76&rateplan=937fa546-fec5-fcbc-2b5d-04f22c071a13&usercountry=IN&currency=INR&userdevice=desktop&verif=false&audience_list=&mcid=332&booking_source=cpc&adtype=1&push_id=CgYIgJbnsAYSBgiAueywBhgBIKDy7xIqDBgBKggiAggBKgIIBA%3D%3D937fa546-fec5-fcbc-2b5d-04f22c071a13_20240412_10&gclid=Cj0KCQjwlN6wBhCcARIsAKZvD5g7RTaTN6JjXjGwhXTSIBNj2jEWvioBiR5E6ERoIoKHIBOLpYgYDhwaAkeBEALw_wcB&los=1&adults=2&rooms=1&checkin=2024-04-13&checkout=2024-04-14&selectedproperty=39581984&city=17269&cid=1918349&pslc=1&ds=IUpATh8VkRCiNnAT" title="Laksh Grand Resort">
                    <AREA shape="rect" coords="539,345,667,407" href="https://www.goibibo.com/hotels/meta/google/4354390963378411938/3540257811845764463/%7B%22ci%22:%2220240413%22,%22co%22:%2220240414%22,%22r%22:%221-2_0%22,%22ibp%22:%22v15%22%7D/?hquery={%22ci%22:%2220240413%22,%22co%22:%2220240414%22,%22r%22:%221-2_0%22,%22qd%22:%2220240413-20240414-1-2_0%22,%22ibp%22:%22v15%22}&utm_source=meta&cmp=META|google|cpc_hpa|googlehoteldfinder|Hotel_Price_Ads_3540257811845764463|META&utm_medium=cpc_hpa&utm_campaign=Hotel_Price_Ads_19905350044_3540257811845764463&vendor=gds&p=1636.40&c=INR&bookingSource=commissions&adType=1&gclid=Cj0KCQjwlN6wBhCcARIsAKZvD5iq5W5ntjSqfMfzNq0F0wSaCOn3dwkJw3Tig3aqE1EUBWPbvzKjAhcaArdQEALw_wcB" title="Country club Lee Crysstal - Boutique Hotel">
                        <AREA shape="rect" coords="742,162,919,218" href="https://www.makemytrip.com/hotels/hotel-listing/?topHtlId=202109211631562045&city=CTMAA&country=IN&checkin=04132024&checkout=04142024&roomStayQualifier=2e0e&totalGuestCount=2&roomCount=1&cmp=googlehoteldfinder_DH_META_Paid_selected_IN_mapresults_202109211631562045&_uCurrency=INR&Campaign=20607960138&locusId=CTMAA&locusType=city&mtkeys=3ea0338e-cf36-453a-bc7c-c382698d6ca7&au=&gclid=Cj0KCQjwlN6wBhCcARIsAKZvD5gWDllpXvek6_tZCDcm1sRYgZE-3w3I1jYg2b3tZrbNOFVXFiORQK4aAhM3EALw_wcB" title="Le Grace chennai ECR">
                            <AREA shape="rect" coords="1102,397,1302,447" href="https://www.goibibo.com/hotels/meta/google/4354390963378411938/9148435948091139586/%7B%22ci%22:%2220240413%22,%22co%22:%2220240414%22,%22r%22:%221-2_0%22,%22ibp%22:%22%22%7D/?hquery={%22ci%22:%2220240413%22,%22co%22:%2220240414%22,%22r%22:%221-2_0%22,%22qd%22:%2220240413-20240414-1-2_0%22,%22ibp%22:%22%22}&utm_source=meta&cmp=META|google|cpc_hpa|googlehoteldfinder|Hotel_Price_Ads_9148435948091139586|META&utm_medium=cpc_hpa&utm_campaign=Hotel_Price_Ads_19905408880_9148435948091139586&vendor=&p=21186.90&c=INR&bookingSource=commissions&adType=1&gclid=Cj0KCQjwlN6wBhCcARIsAKZvD5iVKB2gnAmkqssixOUUTLRI5VUHnbzeIEoIB9OKpfHmnlCtRsgHHs4aApKbEALw_wcB" title="Mer Vue Villa (Beach house)">
                                <AREA shape="rect" coords="1076,69,1220,112" href="https://www.agoda.com/search?campaignid=21176660567&searchdatetype=selected&lt=1&numberofchildren=0&childages=&gsite=mapresults&partnercurrency=INR&roomid=565105220&pricetax=183.60&pricetotal=1713.60&rateplan=85baaefd-ec1c-e203-6ca2-f8eb2c1cb9fb&usercountry=IN&currency=INR&userdevice=desktop&verif=false&audience_list=&mcid=332&booking_source=cpc&adtype=1&push_id=CgYIgJbnsAYSBgiAueywBhgBINymhAEqDBgBKggiAggBKgIIBA%3D%3D85baaefd-ec1c-e203-6ca2-f8eb2c1cb9fb_20240412_10&gclid=Cj0KCQjwlN6wBhCcARIsAKZvD5g9nlLSTab6PdGHzDlDE_O3sPX4chFt2OcJ6MSwmuQdiKuXjwJ9wcwaAkkYEALw_wcB&los=1&adults=2&rooms=1&checkin=2024-04-13&checkout=2024-04-14&selectedproperty=2167644&city=17269&cid=1918349&pslc=1&ds=lMZDA4D1wPuieZNR" title="Grand Bay resort">
        </MAP>
        <br>
        X-coordinate
            <input type="text" id="Text1">
        Y-coordinate 
            <input type="text" id="Text2">
</body>
</html>
```

## OUTPUT

![Screenshot 2024-04-12 103021](https://github.com/selvasachein/NearMe/assets/130027697/fef756f9-df18-4b13-a19d-75d1dfaf613b)


![Screenshot 2024-04-12 103040](https://github.com/selvasachein/NearMe/assets/130027697/712588a0-8e35-4040-ae63-a71ee75d2354)

![po](https://github.com/selvasachein/NearMe/assets/130027697/b9bdee86-567a-4b37-bea5-dd2a8fb833b8)
![Screenshot 2024-04-12 104034](https://github.com/selvasachein/NearMe/assets/130027697/fd06f4be-61e3-4bc3-8365-44e95f6d045b)

![oi](https://github.com/selvasachein/NearMe/assets/130027697/d9bb70b4-4e20-48bb-8e28-1753ead8aa76)
![Screenshot 2024-04-12 104205](https://github.com/selvasachein/NearMe/assets/130027697/42a70b64-09c7-4075-a17a-d555eeef40f3)

![iu](https://github.com/selvasachein/NearMe/assets/130027697/ce0d8aa0-619f-4afd-b654-aad4277d0c9f)

![Screenshot 2024-04-12 104218](https://github.com/selvasachein/NearMe/assets/130027697/c6f6cc9d-41a9-438b-84d1-fa2973baf5e4)

![uy](https://github.com/selvasachein/NearMe/assets/130027697/73e5aa41-de6f-4d45-9ffa-904518a78068)

![Screenshot 2024-04-12 104238](https://github.com/selvasachein/NearMe/assets/130027697/5823b27d-ea67-40fd-8bae-14d74b20cc1a)

![yt](https://github.com/selvasachein/NearMe/assets/130027697/1acd3abf-347b-44b6-a830-dde36048874f)

![Screenshot 2024-04-12 104254](https://github.com/selvasachein/NearMe/assets/130027697/0390ea86-f0b1-4701-91da-dafcce6a469c)


## RESULT
The program for implementing image maps using HTML is executed successfully.
