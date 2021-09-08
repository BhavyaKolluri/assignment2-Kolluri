# assignment2-Kolluri
# Bhavya Kolluri
###### My Favourite place is HYDERABAD in India.
Hyderabad is a historical place with all **Beautiful Monuments**. I lived in Hyderabad for more than 4 years. It is a wonderful experience. It has the perfect blend of modern and cultrually rich india.

***

# Directions to my Faviurite Place from Maryville.
1. Go to Kansas International Airport.
2. Buy Flight ticket to Shamshabad Airport in India.
3. It shows the following terminals through QATAR Airways
    1. Seattle
    2. Doha
    3. Chennai
    4. Hyderabad
1. After reaching Airport in Hyderabad
2. Travel all over the city
3. View all Historical places like
    1. Golconda Fort
    2. Charminar
    3. Salar jung Museum
* Story books
    * Comic books
* puppy
* Pizza
* coke

**[Link to AboutMe.md file](AboutMe.md)**

***

# Food/Drinks Recommended
Following table describes about food/drinks. My personal choice would be Chicken spicy burger which is available in Mc Donalds,Redbull from Walmart,Thin crust pizza from Pizzahut are delicious and a Diet coke which also available in Mc Donalds.

|  food/drink(item)         |   location   |   price   |
| ------------------------- | ------------ | --------: |
| Chicken spicy burger      |   Mc Donalds |   $5.99   |
| Red Bull                  |   Walmart    |   $1.00   |
| Thin crust pizza          |   Pizzahut   |   $10.00  |
| Coke                      |   Mc Donalds |   $7.99   |

***

# My Favorite Quotes

> Never trouble troublw till trouble troubles you - *Bruce Lee*

> I want to be somebody. I mean I AM somebody, I just want to be a RICH somebody - *Octavia St. Laurent*

***

# Alogorithm of Graphs Traversal
> Breadth-first search(BFS) is an algorithm for searching a tree data structure for a node that satisfies a given property. It starts at the tree root and explores all nodes at the present depth prior to moving on to the nodes at the next depth level. Extra memory, usually a queue, is needed to keep track of the child nodes that were encountered but not yet explored.
Read More <https://en.wikipedia.org/wiki/Breadth-first_search>
~~~
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
~~~
For More information <https://cp-algorithms.com/graph/breadth-first-search.html>