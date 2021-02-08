Homework No. 1
================
Victor H. Ramirez, EID vhr267
February 8, 2021

# 1. Data visualization: gas prices

What drives the differences in the price of gasoline between different
gas stations in the Austin area? According to theory, the final price
charged to the consumers is a consequence of the market forces (i.e.,
supply and demand), geographical differences (e.g., in taxes and other
regulations), and of the market structure, which relates to the market
power of the seller. Since we focus our attention to the Austin area,
geographical differences will not be relevant in this case. On the other
hand, economic variables that potentially affect supply and demand tend
to show a high degree of autocorrelation through time (e.g., an increase
in international oil prices should affect the price of gas for a
relative long period of time, not just when the increment occurs). This
posses a challenge then, since we must be able to disentangle the
effects of different factors varying over time.

To better understand then the differences in prices charged by stations,
we restrict our attention to data from 101 gas stations in the Austin
area in a single point in time (specifically, April 3rd 2016), and
explore the possible effect of a number of potential drivers. Since it
seems reasonable to assume that cost structures and technologies are
quite similar between gas stations, we may ignore supply factors in the
analysis and study factors associated to demand and market structure:

-   Determinants of the demand: household income in the area, search
    costs;
-   Market structure: degree of competition, brand-specific’s
    price-elasticity of the demand.

We start by exploring the effect of direct competition on gas prices.

## 1.a Degree of competition

Gas stations may be analyzed in most scenarios like acting as a monopoly
or an oligopoly. The degree to which a particular gas station may be
considered as one or the other will stem, in part, from conflation of
high research costs (which grow with the distance to the next gas
station) and thus with the presence of direct competitors in the nearby
area.

It is a well established theoretical fact that oligopolies will, in
general, charge a price that is smaller than the price charged by a
monopoly, but greater than the market price under perfect competition
(in most cases). In particular, oligopolies will only reach the perfect
competition price if they engage in a price war. In practice, however,
we expect this to occur only very rarely.

On the other hand, it is very unlikely that oligopolies will reach the
monopoly price. This is because, for once, it is against the law to
collude to set prices, and, in any case, the participants always have an
incentive to increase their own supply (and thus drive prices down).

Figure 1 explores evidence in this sense. The figure presents the
distribution of prices of gas stations according to whether there are
competitors in sight.

![Direct competition drives prices down: although there is considerable
overlap in price distribution, the median price of gas stations with
competitors in sight is lower than that of their
counterparts.](Homework-1-VHRH_files/figure-gfm/unnamed-chunk-2-1.png)

As observed in Figure 1, although there is considerable overlap between
the distributions, the difference in median price charged for gasoline
seems to confirm that there is a direct, negative effect of competition
on price. We explore next the effect of income on gas prices.

## 1.b Income effect

Since gasoline is a complementary good for particular-use automobiles,
and the demand for these expands as the household’s income increases, we
expect that an increment in household income should drive gasoline
prices up.

If this is the case, systematic differences in median household income
for a particular region should translate in regional differences in
gasoline prices. Figure 2 shows prices and median household income per
zip code and confirms that there is a positive relation between between
these variables, as expected.

![Higher income means higher gas prices: there is a direct, positive
relationship between median household income and gas prices per zip
code](Homework-1-VHRH_files/figure-gfm/unnamed-chunk-3-1.png)

## 1.c Brand differentiation

Figures 1 and 2 have shown some evidence in favor of theoretical drivers
of gasoline prices, albeit with in a somewhat noisy manner. It is
possible that some of the variation in prices is a consequence of
characteristics (real or perceived) of the brand or the seller, such as
quality or service. This type of characteristics is important because it
causes the firm’s demand curve to be more inelastic, so sellers might
charge higher prices.

To see if this might be the case, we explore in Figure 3 whether there
is a significative difference between average brand prices. In
particular, we explore whether Shell charges more for gasoline than its
competitors. The Figure shows that this is not the case. Although
Shell’s gasoline is more expensive than that ExxonMobil and other,
unspecified brands, their average price is in fact a little lower than
the Chevron-Texaco’s price. In any case, the average price differences
are negligible.

![Does Shell charge higher prices than their competitors? This is simply
not true, since Chevron-Texaco charges a slightly higher price for
regular
gasoline.](Homework-1-VHRH_files/figure-gfm/unnamed-chunk-4-1.png)

## 1.d Reduced opportunity costs

If it is true that consumer’s costs (other than the gasoline price) play
a prominent role in the demand for gasoline, then it is possible that
gas stations at stoplights should have a higher demand than their
counterparts. This is because, on the one hand, the opportunity cost of
the consumer is reduced when forced to stop near a gas station (“since
we already had to stop, might as well get some gas”) and the acquisition
of information is relatively cheaper as well (there is potentially
enough time to consider prices and to calculate whether one will need to
fill up the tank in the near future in any case).

![Gas stations at stoplights charge more: Although there is significan
overlap in the price distribution, gas stations at stoplights will more
frequently charge slightly higher prices than their
counterparts.](Homework-1-VHRH_files/figure-gfm/unnamed-chunk-5-1.png)
Figure 4 suggests that this is indeed the case. Although the variability
of prices of gas stations not situated at a stoplight is greater, we
observe that the mode of said distribution is of US$1.8/Gallon, while
the mode of the stop-light gas stations is closer to US$1.9/Gallon.

## 1.e Reduced search costs

In the same vein, we should observe that gas stations with more
accessibility from a more transited road should face a higher demand,
first, because the additional gasoline consumption and car depreciation
incurred to search for alternatives make no sense if different brands of
gasoline are considered relatively good substitutes; and second, because
there is the possibility that one is running very low on gas, so the
uncertainty of being able to reach another gas station is eliminated if
we simply fill-up the tank at the closer station. ![Gas stations near
highways charge more for gas: the increased accessibility means that gas
stations of all brands consistently charge more for gasoline when the
station has direct highway
access](Homework-1-VHRH_files/figure-gfm/unnamed-chunk-6-1.png) Figure 5
shows that this is indeed the case for every brand, since prices for gas
stations near highways are consistently higher.

# 2. Data visualization: a bike share network

Bike sharing systems have gained prominence in recent times among
environmentally conscious people and because of the convenience in
cities with heavy traffic.

To appropriately be able to meet the demand for this type of bikes, it
is of great importance that we identify peak hours and other seasonal
patterns. Among the factors that could influence these patterns we could
mention the day of the week and weather conditions. We focus on data
that covers a two year period for the Capital Bikeshare system in
Washington D.C.

First, we explore the average number of bike rentals (totals) vs hour of
the day (hr), shown in Figure 6. We observe that the pattern of usage of
the bikes is very clearly correlated with the start and end of the
workday, since demand peaks at 8:00 a.m. and 5:00 p.m., sith a slump at
12:00 p.m., possibly related to lunchtime.

![Bike rentals per hour of the day: demand increases at the start and
end of the
workday](Homework-1-VHRH_files/figure-gfm/unnamed-chunk-8-1.png)

If the above is true, we should see a different demand pattern for work
vs non-workdays. Figure 7 shows that this is indeed the case, with
demand peaking near noon, but decreases very slowly afterwards.

![Bike rentals demand peaks near noon for non-working days and is more
consistent throughout the day than for working days
(Workingday=1)](Homework-1-VHRH_files/figure-gfm/unnamed-chunk-9-1.png)

To assess the effect of the weather on demand, we focus on a single time
of the day (8:00 a.m.), and difference between working and non-working
days. Figure 8 shows the average demand for weather conditions that go
from best (coded as 1) to worst (scale actually goes to 4, but there are
no occurrences in the sample employed). We observe that, although demand
naturally increases with better weather conditions, the biggest
difference occurs conditional on whether it is a rainy or snowy day.

![Influence of weather on average bike rides: demand decreases
dramatically on rainy and snowy days. This behaviour is consistent in
working and non-working days. (Best weather conditions: weathersit =
1)](Homework-1-VHRH_files/figure-gfm/unnamed-chunk-10-1.png)

# 3. Data visualization: flights at Austin-Bergstrom International Airport

What is the best time of the day to fly to minimize delays at the
Austin-Bergstrom International Airport (ABIA)? This question is more
complex than it might seem at first, as will be shown below.

To begin with, it is not clear weather one would be more concerned with
departing or arriving on time. To the degree that flight conditions are
consistent, these two variables should be very correlated. To see if
this is the case, we construct Figure 9, which plots Arrival vs
Departure delays. The figure shows that, specially for long delay times
(which would be our main concern), these variables are very strongly
correlated, so we may indifferently employ one or the other in the
analysis and simply refer to it as “Delays”.

![Departure and arrival delay time correlation increases with delay time
(minutes).](Homework-1-VHRH_files/figure-gfm/unnamed-chunk-12-1.png)

Now, there are many reasons why a flight may be delayed. It could be
that there are mechanical issues with the plane that must be corrected.
It could alternatively be that the weather conditions are not good
enough for take off, so there are groups of delayed flights. In any
case, there are reasons to believe that delay times are autocorrelated
across the time of the day.

Figure 10 shows that the average delay increases slightly with supposed
departure time, although there is still a lot of variability in delay
times.

![Delay times tend to increase with intended departure hour of the
day](Homework-1-VHRH_files/figure-gfm/unnamed-chunk-13-1.png)

Figure 11 shows that this is indeed the case, as the median delay time
increases from less than 5 minutes at 5 a.m., to almost half an hour at
11 p.m.

![The median delay time increases from approximately 5 to 30 minutes
throughout the
day](Homework-1-VHRH_files/figure-gfm/unnamed-chunk-14-1.png) It could
be that these times differ by airline. In the data, there are 16 unique
carriers; however, Table 1 shows that the most frequent flights are by
far American Airlines (AA) and Southwest Airlines (WN), so we will focus
on delay times of these to carriers.

    ## ### Frequencies  
    ## #### ABIA$UniqueCarrier  
    ## **Type:** Character  
    ## 
    ## |    &nbsp; |  Freq |      % |
    ## |----------:|------:|-------:|
    ## |    **9E** |  2549 |   2.57 |
    ## |    **AA** | 19995 |  20.14 |
    ## |    **B6** |  4798 |   4.83 |
    ## |    **CO** |  9230 |   9.30 |
    ## |    **DL** |  2134 |   2.15 |
    ## |    **EV** |   825 |   0.83 |
    ## |    **F9** |  2132 |   2.15 |
    ## |    **MQ** |  2663 |   2.68 |
    ## |    **NW** |   121 |   0.12 |
    ## |    **OH** |  2986 |   3.01 |
    ## |    **OO** |  4015 |   4.04 |
    ## |    **UA** |  1866 |   1.88 |
    ## |    **US** |  1458 |   1.47 |
    ## |    **WN** | 34876 |  35.14 |
    ## |    **XE** |  4618 |   4.65 |
    ## |    **YV** |  4994 |   5.03 |
    ## | **Total** | 99260 | 100.00 |

Figure 12 confirms that this trend repeats itself for the two principal
airlines; but that delay times are consistently lower for Southwest
Airlines throughout the day. We conclude that, as it is very likely that
one should travel with American or Southwest Airlines through the ABIA,
in order to avoid potential long delay times, it is advisable to fly
early in the morning with Southwest Airlines.

![Delay times increase through the day for American and Southwest
Airlines, the delay times for American Airlines are consistently
greater,
however.](Homework-1-VHRH_files/figure-gfm/unnamed-chunk-16-1.png)

# 4. k-nearest neighbors

We are interested on estimating a non-parametric model to forecast the
market price of a Mercedes Benz S Class, based on one of its many
characteristics: its mileage. In particular, we have information on two
S Class Mercedes Benz according to the car’s trim level: the 350 and 65
AMG, and want to employ the K-nearest neighbors algorithm to obtain our
forecast. This algorithm necessitates that we specify the number K of
points used in the training data. With this in mind, we will proceed by
first filtering out these trim levels to better understand the
relationship that the price of each one of them and their mileage. This
step is important because the apparent degree of “linearity” of the data
will be determinant in the value of K to choose. Figure 13 shows price
vs mileage for the two types of vehicle.

![Price decreases exponentially with car
mileage](Homework-1-VHRH_files/figure-gfm/unnamed-chunk-18-1.png)

The above figure shows that the car of the price decreases exponentially
with mileage. This makes sense: when the new car leaves the dealer, it
is automatically and rapidly depreciated; but the mileage is
subsequently more related to the overall condition of the car and less
to its depreciation as mileage increases. This considerations imply a
low value of k, since we need enough flexibility to capture the
nonlinear relationship between price and mileage.

The figure also shows very evidently that there are two types of the
S350 models. This makes it harder to provide accurate predictions of the
price for the mileage values where the structural break occurs (25000 to
75000 miles), and could be result of a discontinued model in the data.
As a consequence, we would prefer a bigger value of k, so that price
predictions don’t jump erratically as we consider close mileages.

Now, we must establish the feasible limits for the k parameter. Since,
after filtering out these two trims, we retain 416 and 292 observations
for the 350 and 65 AMG trim, respectively, and because we employ
training sets that take 80% of the data we cannot exceed values of k of
around 300 and 200.

Second, we must take into account that the out-of-sample RMSE for a
particular value of k is a random variable in itself, thus, it is
necessary to assess the quality of our guess. To this end, we may obtain
repeated samples with each value of k and estimate the RMSE, to
construct the distribution of the estimate. Figure 14 shows box plots
for several possible values of k. We observe that the average RMSE of
the out-of-sample predictions is minimized at values of 10 for both.

![RMSE distribution of out-of-sample predictions with KNN models with
different values of k. results based on 1000 replications for each k
value](Homework-1-VHRH_files/figure-gfm/unnamed-chunk-19-1.png)

This is not surprising if we consider the similarities in the relation
between price and mileage for both types of car (that is, an exponential
relationship); it has the consequence, however, of getting the unwanted
effect of erratic jumps in the price forecast for the 350 trim. Figure
15 shows this effect.

![KNN Models forecast of price as a function of
mileage.](Homework-1-VHRH_files/figure-gfm/unnamed-chunk-20-1.png)

The effect seems to be problematic for mileages between 50000 and 75000,
but is appropriate otherwise. The “wigglines” of the predictions seems
to be characteristic of this methodology, however, as observed in the
right panel of Figure 15.
