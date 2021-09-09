# assignment2-thodati
## Thodati Sai Chandhar Reddy
   paris
   Because of its **vibrant** tourist **spots**


   ***
   ## Route to Hyderabad
   1. Take a roadway from Maryville to Kansas airport.
   2. Take a fight to biggest airports like New york, Chicago, Dallas etc... Let's say New york.
   3. Take a fight either directly to Delhi or else through London, Doha, Germany etc to Delhi.
   4. From there we can go by train which will be 12 hours journey or take a flight which hardly take one and half hour  

   ## List of items to take
   - Camera
   - Favourite food items like sweets, chocolates etc
   - cloths

   [About me](/AboutMe.md)

   ***
   ## Information about foods and drinks
   The following table consists of food/drinks, location and price

|food/drinks           | Location                  |  amount    |      
| ---------------------| --------------------------| -----------|
| chicken biryani      | KS biryani center,Kansas  |  $17       |
| mutton pulusu        | Dawwath, Dallas           |  $23       |
| Fish fry             | Indian recipie, Kansas    |  $18       |
| Egg fried rice       |Indian recipie, Kansas     |  $10       |
   
## Quotes
>Intelligence is the ability to adapt to change.

   -*Stephen Hawking*


>Death is so terribly final, while life is full of possibilities.

   -*George R.R Martin*

   ## Code fencing


   >Breadth First Traversal (or Search) for a graph is similar to Breadth First Traversal of a tree (See method 2 of this post). The only catch here is, unlike trees, graphs may contain cycles, so we may come to the same node again. To avoid processing a node more than once, we use a boolean visited array. For simplicity, it is assumed that all vertices are reachable from the starting vertex.

   [Introduction](https://www.geeksforgeeks.org/breadth-first-search-or-bfs-for-a-graph)


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
  [code link](https://cp-algorithms.com/graph/breadth-first-search.html)