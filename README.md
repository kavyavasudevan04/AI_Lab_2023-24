# AI_Lab_2023-24
LAB EXPERIMENTS 
# REQUIREMENTS 
1. PYHTON
2. SWI-PROLOG
3. PDDL 0R PDDL EDITOR ONLINE
4. JUPITER OR COLAB NOTEBOOK

# Program: 
graph = {
 '5' : ['3','7'],
 '3' : ['2', '4'],
 '7' : ['8'],
 '2' : [],
 '4' : ['8'],
 '8' : []
 }
 visited = [] 
 queue = []     
 def bfs(visited, graph, node): 
 	 visited.append(node)
  	queue.append(node)
  		while queue:          
    			m = queue.pop(0) 
    			print (m) 
    			for neighbour in graph[m]:
      				if neighbour not in visited:
        					visited.append(neighbour)
       					 queue.append(neighbour)


print("Following is the Breadth-First Search")
bfs(visited, graph, '5')

# Output:

