**1.	TO WHAT EXTENT DOES TRAFFIC DENSITY CONTRIBUTE TO THE COST OF LIVING INDEX, AND ARE THERE SPECIFIC CITIES WHERE THIS IMPACT IS MORE PRONOUNCED?
**
In the SELECT statement of my query, i specified relevant columns, Cost of Living Index and Traffic Density. I also included City to identify how cities fare against those 2 variables. Using the ORDER BY function, I further organized the cost of living index in DESC order in order to establish how cities with the highest cost of living indexes fared against Traffic Density listed as low medium and high. The results showed that cities with high traffic density have a low cost of living index while those with high traffic density have a high cost of living index

**2.	IS THERE A DISCERNIBLE PATTERN BETWEEN AIR QUALITY INDEX AND HAPPINESS SCORE, AND HOW DOES THE PRESENCE OF GREEN SPACES INTERACT WITH AIR QUALITY IN INFLUENCING HAPPINESS?
**
In my query, I used the CORR function 3 separate times for the 3 pairs of columns i.e. happiness score and air quality index, happiness score and green space area, air quality index and green space area. The results were 0.3395, -0.9954 and -0.4092 respectively indicating a positive linear relationship, strong negative linear relationship and moderate negative linear relationship respectively

**3.	HOW DOES THE RELATIONSHIP BETWEEN AIR QUALITY INDEX AND HEALTHCARE INDEX VARY AMONG THE VARIOUS CITIES?
**
In the query's SELECT statement, I input relevant columns such as city, air quality index and healthcare index. Following that, I used the ORDER BY function to arrange the output of Air quality index in ASC order and applied a LIMIT of 5. Subsequently, i applied a UNION ALL to combine the results with a second query whose SELECT statement had the same columns except that the ORDER BY function for air quality index was set to DESC order with a LIMIT of 5.

The results indicate that countries with the highest air quality (which indicates poorer quality air) also have a low health care index. Conversely countries with the lowest air quality index have a high health care index

**4.	DO CITIES WITH MORE GREEN SPACE AREAS HAVE A BETTER HEALTHCARE INDEX? 
**
Just like the query in 3) above, I input relevant columns such as city, green space area and healthcare index. I utilized the ORDER BY function to arrange the green space area in ASC order and applied a LIMIT of 5. Subsequently, i applied a UNION ALL to combine the results with a second query which specified the same columns in the SELECT statement. However, the ORDER BY function for green space area was set to DESC order with a LIMIT of 5 as well.
The cities with highest green space areas have a very high health care index while those with the lowest green space areas also have very low health care index. This indicates a positive linear relationship between green space areas and health care index This result is validated by a subsequent query which returns a value of 0.4543 thereby proving the existence of a positive linear relationship albeit a moderate one.

**5.	ARE THERE NOTICEABLE TRENDS IN THE HAPPINESS SCORE OVER THE YEARS? 
**
In the SELECT statement of the query, I specified the year column and calculated the AVG of the happiness score for all the years. Thereafter I ordered by and grouped by the years.
The results indicate that over the years starting from 2023 to 2029 the average happiness score continually declines.

**6.	WHAT IS THE AVERAGE DECIBEL AND WHICH CITIES ARE ABOVE AVERAGE? 
**
In this case, i developed a nested query to find the solution. The inner query first calculated the AVG decibel level while the outer query used the WHERE function to establish decibel levels greater than the average. To manage the output, i used the ORDER BY function to arrange the decibel levels in DESC order and applied a LIMIT of 10.
The cities listed (Karachi, New Delhi, Bangalore, Jakarta, Hanoi, Islamabad, Mumbai, and Manila) are from South Asia and Southeast Asia regions. The reasons for higher than average decibel levels could be due to population density, traffic congestion and industrial activities. 





