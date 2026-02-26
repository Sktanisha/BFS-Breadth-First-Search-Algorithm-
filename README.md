Description: 
Here, we need to find the path and cost from the source to the destination. To solve the problem, we have taken an adjacent list and a queue. 
Initially, the distance of all nodes is 0. If a vertex is pushed to the queue, the number of visited value become 1. After pop the node from the queue, the adjacence nodes are pushed to the queue of that node. 
Pseudocode: 
visit[source] = 1; dist[source] = 0; // initialization of visit and distance 
Q.push(source); // push the source node to the queue
while(!Q.empty())
      int node = Q.front();
       Q.pop();
for i to graph[node].size() // for loop to check and push the adjacent nodes
       int next = graph[node][i];
           if(visit[next] == 0;
                visit[next] == 1;              //visiting
                dist[next] = dist[node] + 1;   //update
                Q.push(next);                  //push to queue
            
Findings:
•	The BFS algorithm can be applied to both directed and undirected graphs. 
•	It doesn’t follow a long path.
•	This algorithm gives the minimal or the shortest path.
Limitations:  
•	This algorithm consumes more memory.
•	Time complexity is high.
•	If the search space is large, the performance will be poor. 
