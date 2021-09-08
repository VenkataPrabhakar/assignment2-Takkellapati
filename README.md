# assignment2-Takkellapati
# Venkata Prabhakar
###### Paris. Eiffel Tower at night 
__Paris. Eiffel Tower__ Paris is yet untouched by the skyscrapers that dominate the __skylines of London__ and New York, so take advantage of the beautiful Eiffel Tower views you can catch from almost anywhere in the city.


***
###### DIRECTIONS FROM MARYVILLE TO MY FAVOURITE PLACE
1. Distance from maryville to paris is 4478 mi.
2. Total journey time on average 14hours.
3. Take a flight from kansas to dallas.
4. Connect flight to dallas to paris.

###### Enjoyable Moments
* A lot of time spent nearby eifel tower by roaming over there.
* Enjoyed Trocadéro at sunrise.
* Colonnes de Buren For the best photos.
* Musée de l’Orangerie the fabulous pavilion of the Orangerie Museum.
***
###### It Navigates to About.Md file

![Description_AboutMe](https://github.com/VenkataPrabhakar/assignment2-Takkellapati/blob/337a2c090326d8fc8d314f8116394adb78a82ed1/AboutMe.md)

***

The table below describes about food items and its cost.

| food/drinkl          | Location      |  Amount       |
| :---                 |    :----:     |          ---: |
| Pizza                | Pizzahut      | $14.56        |
| Chicken Wings        | Pizzahut      | $13.26        |
| Mexican Tacos        | Taco Bell     | $07.45        |
| Blackcurren icecream | Krish&Kate    | $3.99         |

***

#Pithy Quotes
> The greatest glory in living lies not in never falling, but in rising every time we fall. *-Nelson Mandela*

> he way to get started is to quit talking and begin doing. *-Walt Disney*

***
# Code Fencing

> Graph traversal is a technique used to search for a vertex in a graph. It is also used to decide the order of vertices to be visited in the search process (https://www.educative.io/edpresso/graphs-basics-representation-traversals-and-applications)

```
vector<vector<int>> adj;  // adjacency list representation
int n; // number of nodes
int s; // source vertex

queue<int> q;
vector<bool> used(n);
vector<int> d(n), p(n);

q.push(s);
used[s] = true;
p[s] = -1;
while (!q.empty()) {
    int v = q.front();
    q.pop();
    for (int u : adj[v]) {
        if (!used[u]) {
            used[u] = true;
            q.push(u);
            d[u] = d[v] + 1;
            p[u] = v;
        }
    }
}

```