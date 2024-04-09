# Key Points
- Alg is a process.
- Alg already created before someone else, just we followed those instructions.
# Tree vs Graph
- Graph is parent, tree is children.
- Graph is bigger than tree.
- Tree is a part of graph.
- Graph has no root, but tree has a root.
- Graph node hase multiple edge, tree node only one edge.
- Graph has multiple way to traverse a node, tree only one way to traverse a node.
- Graph possible cycling, tree not possible.
- Graph edge directions can possible both of way parent to children, children to parent, but tree edge directions only one way parent to children.
- Tree is a under of Graph.
# Types of Graph
- Undirected Graph
- Directed Graph
- Weighted Graph
- Unweighted Graph
- Cycle Graph
# Graph Representation
- Must have two things:
	- Number of Nodes(N)
	- Number of Edges(E)
	- Values of Nodes (N-1)
- Three ways graph representation:
	- Adjacency Matrix:
		- Use cases:
			- int mat\[n]\[n]
			- initialy zero(0) filled of cell means not connected.if connected now fill with one(1). ==For unweighted graph==
			- initialy zero(0) filled of cell means not weight and not connectd. if connected now fill with weighted values(value). ==For weighted graph.
			- I will give you two nodes(node1,node2). Now Instantly told me if there are connected or not. ==mat\[node1]\[node2] == 1== . Time complexity O(1)
			- If possible self connected then use.===if(i == j) mat\[i]\[j] = 1.
			- Not use for fined out a node connected how much. Because landy process for find out. but possible.
	- Adjacency List:
		- Use cases:
			- vector\<int> adj[n]
			- Uses for instantly told how many nodes connected a node==unweighted graph==. value are store with stl pair for ==weighed graph==
			- ==for(int i=0; i<adj[3].size(); i++)
	- Edge List:
		- Use cases:
			- vector\<pair<int,int>> edge_list
			- uses to get pair of edge list
https://csacademy.com/app/graph_editor/