# SI 507 2022 Fall

## Introduction




## Preparation
- Yelp Fusion API: `https://api.yelp.com/v3/businesses/search?`
Visit `https://www.yelp.com/developers/documentation/v3/authentication` to get your own API Key. Replace the `API_KEY` in the `Final.py` file to run this project. Here is a `tutorial` which will be helpful to apply for the API KEY:
`https://spectralops.io/blog/yelp-api-guide/`
- Wikipedia web: `https://en.wikipedia.org/wiki/List_of_United_States_cities_by_population`
- Mapbox TOKEN: Access this link below to get a mapbox token to creat restaurant maps. `https://www.mapbox.com/`
Replace `MAPBOX_TOKEN` with your key and run the program.

## Data Structure
Tree data structure. The leaf node will be the information of restaurants, the attribute node will be the restaurants attribution.
Every time run the python code, will reorganize the data (stored in cache or requested from web) into a tree as shown below:

![Alt text](https://drive.google.com/file/d/1aiAmACQnSK98GQ5pvgISrV3PNbxdvs2m/view?usp=sharing)

## Demo
https://youtu.be/7m7OKD7_wHI

## Interaction
### Required Package:
- Beautiful Soup; Requests; Webbrowser; plotly
### Get Start:
#### STEP: Finish the Preparation Part
#### STEP: Run Program:
- `First` Question:
    1. See the information of large cities.
    2. Directly search the resturants of a city.
    - If choose 1
        - `Second` Question: Please choose the number of cities you want to see: (Input a number < 326, so that the program will give you a city list with number size of entries)
        - `Third` Question: Please choose the city you want to see (input number): (In the city list, there wil be a rank number. In put the rank number of the city which you want to search)
        - `Forth` Question: Do you want to see the map of this city and the locations of resturants(y or n)? (input Yes, YES, y, Y, YEs, etc. all is okay)
            - If yes, a map figure will pop up, with the marker which contains the information of restaurants distributed in in the map.
            - If no, move to the Fifth Question.
        - `Fifth` Question: Do you want search the resturants through Price and Rate?(y or n)
            - If yes, move to the next question:
                - `Sixth` Question: Which price level do you wnat to see? ($, $$, $$$, $$$$ or No price) (Input one of string)
                - `Seventh` Question: Which rate level do you want to see? ('above 4', 'above 3', 'above 2', 'below 2') (Input one of string)
                - Generate a list contains the information of restaurants under the limitation of sixth and seventh questions.
                    - `Eighth` Question:please input a num of resturant which you want to see the website:(Input the restaurant number, the program will show corresponding website) (If yhe list of restaurant is empty, this question will not pop up)
            - If No, move to the First Question.
    - If choose 2
        - `Ninth` Question: Please enter the city you want to check: (enter the city name: e.g. Ann Arbor, San Jose, etc.)
            - `Forth` Question: Do you want to see the map of this city and the locations of resturants(y or n)? (input Yes, YES, y, Y, YEs, etc. all is okay)
                - If yes, a map figure will pop up, with the marker which contains the information of restaurants distributed in in the map.
                - If no, move to the Fifth Question.
            - `Fifth` Question: Do you want search the resturants through Price and Rate?(y or n)
                - If yes, move to the next question:
                    - `Sixth` Question: Which price level do you wnat to see? ($, $$, $$$, $$$$ or No price) (Input one of string)
                    - `Seventh` Question: Which rate level do you want to see? ('above 4', 'above 3', 'above 2', 'below 2') (Input one of string)
                    - Generate a list contains the information of restaurants under the limitation of sixth and seventh questions.
                        - `Eighth` Question:please input a num of resturant which you want to see the website:(Input the restaurant number, the program will show corresponding website) (If yhe list of restaurant is empty, this question will not pop up)
                - If No, move to the First Question.

    - If exit: exit the program.



