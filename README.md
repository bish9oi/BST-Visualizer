Binary Tree Visualization

Add and search for nodes in a binary tree with an easy-to-use, web-based visualization


![Project Logo](photos/balanced.png)

What is a Binary Tree

A binary tree is a data type where every node in the graph can have at most two children. The node to the left of any parent node must contain a value less than the value of the parent node, and the node to the right must contain a value greater than the value of the parent node.

![Project Logo](tree.PNG)


Using the Visualization

When the visualization is first opened, the screen will be empty





![Project Logo](photos/blank.PNG)


To add a node to the tree, click the Add button, and enter an integer for the new node to hold. Watch as the animation adds the node to the tree. In this case, green represents the node that was just added. To pan on the visualization, click and drag. To zoom in and out on the visualization, scroll up or down.

![Project Logo](photos/singlenode.PNG)


Click the Add button a few more times to add more nodes to the tree, and watch as their insertion is animated. To make the animation progress faster, move the Animation Speed slider farther to the right. Blue represents nodes that must be visited to insert the node into the correct location

![Project Logo](photos/manynodes.PNG)

To watch the binary tree search for a value in itself, slick the Search button, and enter an integer that you previously inserted into the tree. Blue represents nodes that must be visited to find the value, red represents sections of the tree where the value will not be found, and green represents the node that was being searched for. Note that if no node is green, the value was not found.

![Project Logo](photos/search.PNG)





To clear the entire tree, click the Clear button. This will make your screen appear as it did when the visualization was first opened

Rather than manually adding nodes, you can fill the entire tree with a certain number of nodes. To do this, click the Fill button, enter the desired number of nodes in the prompt, and watch as nodes are added one at a time. Note: this clears the current tree

If you do not want to wait for the insertion animation, click the Quick Fill button, which functions the same as the Fill button, but does not animate the insertion process. Note: this also clears the current tree

![Project Logo](photos/fill.PNG)

Code Structure

Node.js - Defines the Node class, the building block of the binary tree. Nodes store their value, references to both of their child nodes, and information to to draw them on-screen (e.g. x and y-coordinates, colors, etc.)

Tree.js - Defines the Tree class, which serves as both a wrapper for the root node of the binary tree (e.g. providing functions for searching the tree for values), and the primary class responsible for animating the binary tree

Controls.js - Defines the Controls class, which connects the buttons (e.g. Clear, Quick Fill, etc.) to the animation functions of the Tree class

Explorer.js - Defines the Explorer class, which adjusts the size and position of the tree to allow for panning and zooming over the entire tree

sketch.js - Instantiates all the necessary objects to run the visualization

See each file for more detailed documentation, and in-depth explanations of how each class functions






# 🌳 Binary Tree Visualization

📌 **Add and search for nodes in a binary tree with an easy-to-use, web-based visualization.**

![Binary Tree Visualization](photos/balanced.png)

---

## 📖 What is a Binary Tree?

A **Binary Tree** is a data structure where every node can have at most **two children**:
- The **left child** contains a value **less than** the parent node.
- The **right child** contains a value **greater than** the parent node.

![Binary Tree Structure](tree.PNG)

---

## 🎯 Features
✅ **Insert Nodes** - Dynamically add nodes to the tree.  
✅ **Animated Visualization** - Watch real-time animations of node insertion and searching.  
✅ **Search Functionality** - Find any value in the tree with visual indicators.  
✅ **Pan & Zoom** - Navigate the tree easily.  
✅ **Speed Control** - Adjust animation speed with a slider.  
✅ **Quick Fill** - Instantly populate the tree with random values.  
✅ **Clear Tree** - Reset the visualization instantly.  

---

## 🚀 Using the Visualization

### 🏁 Initial Screen
When you first open the visualization, the screen will be **empty**.

![Blank Screen](photos/blank.PNG)

### ➕ Adding Nodes
1. Click the **Add** button.
2. Enter an integer value for the node.
3. Watch the node being added with an animation.
   - 🟢 **Green** represents the newly added node.
   - 🔵 **Blue** represents visited nodes while finding the correct position.

![Single Node](photos/singlenode.PNG)

### 🔍 Searching for a Value
1. Click the **Search** button.
2. Enter a number previously inserted.
3. The tree highlights the search path:
   - 🔵 **Blue** - Nodes visited during search.
   - 🔴 **Red** - Paths where the value was not found.
   - 🟢 **Green** - Node found.

![Search Animation](photos/search.PNG)

### 🔄 Filling the Tree
- Click **Fill** to populate the tree with a specified number of nodes.
- Click **Quick Fill** for an **instant** fill without animations.

![Fill Tree](photos/fill.PNG)

### 🗑️ Clearing the Tree
Click the **Clear** button to remove all nodes and reset the visualization.

![Many Nodes](photos/manynodes.PNG)

---

## 🛠️ Code Structure

📂 **Project Files Overview**

| File Name | Description |
|-----------|------------|
| `Node.js` | Defines the `Node` class, storing values, child nodes, and display properties. |
| `Tree.js` | Implements the `Tree` class, handling insertion, searching, and animations. |
| `Controls.js` | Manages UI interactions, connecting buttons to tree functions. |
| `Explorer.js` | Handles panning and zooming for better visualization control. |
| `sketch.js` | Initializes and runs the visualization. |

---

## 📌 Installation & Usage

1️⃣ Clone the repository:
```sh
 git clone https://github.com/your-username/binary-tree-visualization.git
```

2️⃣ Open the project folder:
```sh
 cd binary-tree-visualization
```

3️⃣ Open `index.html` in your browser to start the visualization.

---

## 🎨 Screenshots
| Insertion Animation | Search Visualization |
|---------------------|---------------------|
| ![Insert](photos/singlenode.PNG) | ![Search](photos/search.PNG) |

---

## 💡 Future Improvements
🔹 Enhanced **color customization** for better user experience.  
🔹 Implementing **AVL Tree balancing** feature.  
🔹 Adding **user-defined traversal** options.  

---

## 📝 License
This project is licensed under the **MIT License**. Feel free to use and modify it!

📩 **Feel free to contribute and make this visualization even better!** 🚀



Built with
p5.js - A library for creating visualizations using the canvas
Future Ideas
Make the tree self-balancing using AVL tree rotation
Add an animation for removing a node from the tree
Improve the performance of the Explorer class for larger trees with svg
