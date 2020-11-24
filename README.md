# Ex1
java project Ex1 OOP


 hashMap<node_info,integer>this is the graph
Hashmap<vertix,HashMap<neighbors,weight>>   this is list of neghbors and their weight


public interface weighted_graph {
 
we ask is contains in the graph if not return null
if is exist return the info

   

 public node_info getNode(int key);

first we check if the nodes is in the graph
then we check on the nebors if the edge is exist
 
    public boolean hasEdge(int node1, int node2);
  
first we check if the nodes is in the graph
then we check on the nebors if the edge is exist
 return node1 adge or node2 adge
   
    public double getEdge(int node1, int node2);
   
if the node exist we dont do nothing
if is not exist we do new node and put the value in the node

    public void addNode(int key);
first we check if the nodes is on the graph 
then we see if is connected or not
then if is connect we just change the w
if is not connect we put the w and we give them the value in the nebiros 
   

    public void connect(int node1, int node2, double w);
   
return the collection 

    public Collection<node_info> getV();
  if the id exist 
then if the exist we go to neibors and give all the nebors of this node_id

     
    public Collection<node_info> getV(int node_id);
first we check if the key exist on the graph
we go to the all nebors on this key and delete
then we delete all nebors from him in the same time    

     
    public node_info removeNode(int key);
    
first we check if node in the graph 
then we see if exist between node and node2 adge
then we remove the adge we going to node1 and remove from the nebors node2 them same things on node2 and node1 
     
    public void removeEdge(int node1, int node2);

return node size
    public int nodeSize();
return adge size
    public int edgeSize();
reurn mc 
    public int getMC();
}

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

	i take the graph from  weighted_grap
graph

                                                              

public interface weighted_graph_algorithms {
return the g	

    public void init(weighted_graph g);

return g

    public weighted_graph getGraph();
   return copy of graph
   
    public weighted_graph copy();
first we see if i have adge
then i do hashmap he save for me color and the and node info
then i get all the vectios in the graph and put them on hashmap then i change the color to white
then i take one v and check the nebors and change the color
and after i change all the color then i chack if some of the vecteros is white if not is true if yes is false
i use some queue to save the vectios that i want to go wite him to next and to chack

    public boolean isConnected();
    
     
first we see if i have adge
then i do hashmap he save for me color and the and node info
i save the src and the end in dif new node_indo
then i get all the vectios in the graph and put them on hashmap then i change the color to white
then i take the src and check the nebors and change the color
i use some queue to save the vectios that i want to go wite him to next and to chack
and after i change all the color then i chack if some of the vecteros is white if not is true if yes is false
then i take the some arr[] and put them all  the nebors of on this and i find the min w 
and i do hashmap is call temp to give me all node_info nebors of the same victos that we are on it and put them and with the min i can take the value of this node and i know where to go 
and clear the temp after that
then i have the path in solothion and the w
    public double shortestPathDist(int src, int dest)

first we see if i have adge
then i do hashmap he save for me color and the and node info
i save the src and the end in dif new node_indo
then i get all the vectios in the graph and put them on hashmap then i change the color to white
then i take the src and check the nebors and change the color
i use some queue to save the vectios that i want to go wite him to next and to chack
and after i change all the color then i chack if some of the vecteros is white if not is true if yes is false
then i take the some arr[] and put them all  the nebors of on this and i find the min w 
and i do hashmap is call temp to give me all node_info nebors of the same victos that we are on it and put them and with the min i can take the value of this node and i know where to go 
and clear the temp after that

    public List<node_info> shortestPath(int src, int dest);

    
