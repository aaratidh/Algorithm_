## Algorithm_

This repo include my learning of algorithm. 

##Day_1  # problem solving using Stack in
<!-- MarkdownTOC depth=4 -->
Problem: 
![image](https://user-images.githubusercontent.com/35992124/218293847-af768e34-8f56-4341-b8f4-eb1c442cdc6e.png)

solution: 
![image](https://user-images.githubusercontent.com/35992124/218293808-4f756d4b-da96-4819-955d-1f358d06bd2a.png)

TOP: sort

##Day_2#
<!-- MarkdownTOC depth=4 -->
Problem: Find the most lucrative simple path in a DAG:
![image](https://user-images.githubusercontent.com/35992124/230827737-b99528fe-1659-4add-ae96-b53f405bc94b.png)

Find the  lucrative path from anywher to anywhere in the above DAG:

Algorithm:
Do the topological sort TS in DAG:
for each vertext v in  TS:
   find its nebour one edge far:
        if (the value of the neighbour  is not greater than the sum of value of vertex v and nbr gold )
            update the nbr gold with = (sum of value of vertex v and nbr.gold )
           
repeate untill each and every vertex has been updated in TS list. 

##Day_3 #
<!-- MarkdownTOC depth=4 -->
Find the costliest or Cheapest path in DAG:
Do a topological sort in a graph
set the cost of each vertex cost[vx] = +inf or +inf
set cost[src] = 0
for each vertex v in sorted order (start as src)
      for each nbr of v:
          newcost = cost[v] +edgeWT(V->nbr)
          cost[nbr] = max 0r min (cost[nbr] , newcost)
     cost[vx]:costli(cheap)est path src to vertex


##Day_ 4

##Problem:
<!-- MarkdownTOC depth=4 -->
A binary search tree has been augmented so that each node knows how many tree descendants it
has. (Each node has attributes .key,.d,.lc,.rc ). Write a (recursive) algorithm that is given the root of the
tree and a (0-based) index and that returns the key located at that position in the ordering. So, for
example, if given index 0 it would return the smallest key in the tree.


