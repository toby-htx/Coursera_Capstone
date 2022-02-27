## Capstone Project for the IBM Data Science Professional Certificate

### Aim

Develop an efficient travel plan for tourists in Tokyo by letting them enjoy the most number of experiences in the shortest period of time. Specifically, this plan should allow them to visit Wards whose districts have a high concentration of attractions, food places, and entertainment where it is easy to navigate by foot, and the venues are close to each other.

### Steps and Results

1)  Information about Wards and major districts in Tokyo was scrapped from Wikipedia (https://en.wikipedia.org/wiki/Special_wards_of_Tokyo) using **BeautifulSoup**. **Python’s geopy package** was then used to obtain the latitude and longitude of all the major districts and merged with the former data.
2)  I focused on **data from only the central 5 wards**, or affectionately referred to as the C5W, of **Minato, Shinjuku, Shibuya, Chuo, and Chiyoda**.
3)  I then used the **Foursquare Place API** to generate the top 100 most popular venues and their categories in 1 major district of each Ward.
4)  After some data cleaning, I used the **Folium** library to create a map of Tokyo with the 5 Wards superimposed on it with their corresponding major district.
5)  I clustered the 5 Wards with the **K-Means algorithm** from the Scikit-learn library. 
6)  The **results** indicate that the **Chuo and Minato Wards should be visited by a Tokyo traveler to maximise his experiences in the shortest period of time**.

For a more detailed explanation, please refer to the PDF report.
