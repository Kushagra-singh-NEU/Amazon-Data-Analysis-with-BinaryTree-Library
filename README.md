# Amazon Data Analysis with BinaryTree Library

## Objective

The main objective of this project is to create a BinaryTree library and leverage it for analyzing and visualizing data from an Amazon Prime Video dataset. The BinaryTree library will facilitate efficient data management and exploration through methods like insert, delete, find, and various traversal methods. The Amazon dataset will be used to demonstrate the capabilities of the BinaryTree library in managing and analyzing structured data.

## Project Tasks

1. **Create BinaryTree Library**:
   - Implement a BinaryTree class with methods for data insertion, deletion, searching (find), and various traversal methods (preorder, inorder, postorder).
   - Include functionality to compute the maximum depth of the tree (`max_depth`) and traverse level by level using level-order traversal (`level_order_traversal`) to obtain node lists per level.
   - Implement a method (`max_path_sum`) to determine the highest path sum from any leaf node to the root.

2. **Amazon Dataset Analysis**:
   - Load and preprocess the Amazon Prime Video dataset.
   - Utilize the BinaryTree library to organize and manage the dataset, demonstrating insertions, deletions, and searching operations.
   - Use traversal methods to explore and analyze the dataset, extracting meaningful insights.

3. **Exploratory Data Analysis (EDA)**:
   - Perform EDA on the Amazon dataset using visualization techniques.
   - Generate interactive visualizations to analyze content distribution, trends over time, sentiment analysis, and other relevant metrics.
   - Provide insights into the dataset's characteristics and relationships using the BinaryTree library for data manipulation.

## Main Features

- **BinaryTree**: Efficient management of data using a binary tree data structure.
  - `insert`: Insert new data into the tree.
  - `delete`: Remove data from the tree.
  - `find`: Search for data within the tree.
  - `preorder_traversal`, `inorder_traversal`, `postorder_traversal`: Traverse the tree in different orders.
  - `max_depth`: Compute the maximum depth of the tree.
  - `level_order_traversal`: Traverse the tree level by level.
  - `max_path_sum`: Determine the highest path sum from any leaf node to the root.

- **Amazon Dataset Analysis**:
  - **Price Range Categorization**:
    Use a binary search tree (BST) to categorize products based on their prices. Each node represents a price range, allowing for quick querying and range-based operations.
   
    # Insert price ranges into the BST
    price_bst.insert((0, 10))   # Represents products priced between $0 and $10
    price_bst.insert((11, 20))  # Represents products priced between $11 and $20
    
    # Perform range query
    products_in_range = price_bst.range_query((5, 15))
    print("Products in price range $5 - $15:", products_in_range)

  - **Product Sorting and Searching**:
    Utilize BSTs for efficient sorting and searching of product attributes such as titles, descriptions, or brands.

   # Insert product titles into the BST
    for title in amazon_data['title']:
        title_bst.insert(title)
    
    # Search for a product by title
    product = title_bst.find("Amazon Prime Video")
    if product:
        print("Product found:", product)
    else:
        print("Product not found.")

## Contributors

1. Kushagra Sisodiya
2. Surbhi Wahie 
3. Shrunali Suresh Salian 
4. Harsha Vardhineedi 
