# python-api-challenge
## Part 1 Weather
The purpose of this mini project was to utilize various python libraries to analyze weather across the world in various cities and then using this weather data to look at hotels across the world. pandas, matplotlib, hvplot, citipy and scipy were a handful of the python libraries that were utilized in this project. To obtain the list of cities for looking at the weather random coordinates were obtained using a loop and then cities close to these coordinates were obtained using the citipy library. To access the weather of these random cities the open weather api as accessed. Using this api I was able to obtain various weather stats such as average ax temp and humidity to name a couple. Once all the weather stats were obtained for all the cities, they were put into a dataframe. This dataframe was then turned into a csv file for use in the 2nd part of the project. Various plots were created comparing latitude to various weather stats for all the cities in the dataframe. Then I compared the cities in northern to the cities in the southern hemisphere again using latitude and the various weather stats that were obtained from the open weather api. The plots comparing the cities in northern hemisphere to the southern hemisphere cities also had various statistical stats done on them such as obtaining the correlation value and a linear regression line. Using these statistical test various observations were had on the different weather stats in the two hemispheres. When comparing max temp one relationship was that max temp will most likely be colder if you are closer to either the South or North Pole. There was very little correlation when comparing the humidity of the northern and southern hemisphere. Just like humidity, cloudiness and windspeed had very weak correlation because they had such low r-values. 
## Part 2 Vacation/Hotel
To start the vacation/hotel analysis the csv that was exported in part 1 of this mini project was imported and then turned into a dataframe. This dataframe consisted of the same cities as part 1 of the project and the same weather statistics. Using this dataframe a map plot was created using hvplot each city was displayed on the world map. When hovering over the various cities weather stats would appear as well as the country of the city.  The original dataframe was next filtered based on various criteria of weather that I chose. The criteria I chose was temperature in between 21 to 30 Celsius, Humidity less than 80%, windspeed is less then 4m/s, and cloudiness below 75. This dataframe was then copied and then another column was added for hotel names. A loop was then created that accessed the places geoapify api to find a hotel that was closest to the various cities in the dataframe. This loop iterated through the cities and added the hotel name to the dataframe and if there was no hotel close to the city no hotel name was added. To avoid an error from no hotel existing near the city a try except statement was needed. Using this new dataframe another map plot was created. When hovering over the various cities the hotel name associated with that city would show up as well as the country. 






#Weather Plot Examples 


<img width="626" alt="Screenshot 2024-04-02 at 10 50 07 PM" src="https://github.com/grantgorham26/python-api-challenge/assets/154031840/b79500ba-1287-4278-a586-f6e2c6655d0e">
<img width="640" alt="Screenshot 2024-04-02 at 10 50 15 PM" src="https://github.com/grantgorham26/python-api-challenge/assets/154031840/e164b885-20a2-4a25-b38b-0d7dc076927d">
<img width="626" alt="Screenshot 2024-04-02 at 10 50 25 PM" src="https://github.com/grantgorham26/python-api-challenge/assets/154031840/c5cab76d-92ae-4b41-8235-e9d2c055eb83">
<img width="615" alt="Screenshot 2024-04-02 at 10 50 34 PM" src="https://github.com/grantgorham26/python-api-challenge/assets/154031840/85a339ce-152f-47ad-90c5-98a5b6ab9d86">

#Vacation/hotel Plots
<img width="1031" alt="Screenshot 2024-04-02 at 10 49 32 PM" src="https://github.com/grantgorham26/python-api-challenge/assets/154031840/4bf3f6bf-c267-49f3-b0d7-e4cfa2bf729e">
<img width="1035" alt="Screenshot 2024-04-02 at 10 49 42 PM" src="https://github.com/grantgorham26/python-api-challenge/assets/154031840/9ab51039-c3e5-4431-9886-38077f2ed5ab">











