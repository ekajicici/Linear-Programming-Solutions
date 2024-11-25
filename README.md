### Project Description: Solving Linear Programming (LP) Problems Using Python

In this project, we aim to solve various **Linear Programming (LP)** problems that focus on optimizing resources under given constraints. These problems can be divided into two broad categories: **Maximization** (e.g., maximizing profit, revenue, etc.) and **Minimization** (e.g., minimizing cost, resources, etc.).

#### Objective of the LP Problems

The objective of each linear programming problem is to optimize (maximize or minimize) a certain objective function, subject to a set of constraints. The constraints define the feasible region, and the optimal solution lies at one of the corner points (vertices) of this feasible region. 

For example, in the **Maximizing Profit for a Factory** problem, the objective is to maximize the total profit by deciding how many units of two products to produce, considering the available machine time and raw materials. Each problem has:
- **Decision Variables**: These represent what is being optimized (e.g., the number of products produced).
- **Objective Function**: This defines the goal of the problem (e.g., maximizing profit or minimizing cost).
- **Constraints**: These are the limitations or restrictions (e.g., available labor, materials, machine time).

The key challenges of these problems are to find the feasible region (which satisfies all constraints) and then identify the optimal solution that maximizes or minimizes the objective.

### How the Problems Were Solved

The problems are solved graphically and computationally in Python using the following approach:

1. **Formulation**:
   - Define the **decision variables** (e.g., number of products).
   - Write the **objective function** (e.g., profit or cost) to maximize or minimize.
   - Write the **constraints** (e.g., machine hours, material availability).

2. **Graphical Method** (for 2-variable problems):
   - Plot the **constraints** as lines or inequalities on a graph.
   - **Shade the feasible region** where all constraints are satisfied.
   - Identify the **corner points** (vertices) of the feasible region.
   - **Evaluate the objective function** at each corner point to determine the maximum or minimum value.

3. **Python Libraries Used**:
   - **Matplotlib**: Used for plotting the constraints and feasible region.
   - **NumPy**: Used for efficient handling of numerical data and creating the constraint lines.
   - **SciPy/Linear Programming (Pulp)**: While for graphical solutions, constraints and objectives are evaluated manually, you could also use these libraries for automated LP solvers.

### Step-by-Step Python Code Execution

1. **Defining Constraints**: For each problem, we first define the mathematical constraints based on the problem’s description. These constraints are typically linear equations or inequalities.

2. **Plotting the Constraints**: Using **Matplotlib**, we plot each constraint as a line, and shade the feasible region where all constraints are satisfied. This allows us to visually see the solution space.

3. **Finding Corner Points**: The feasible region is formed by the intersections of the constraint lines. These intersections are the **corner points** of the feasible region.

4. **Evaluating the Objective Function**: We evaluate the objective function at each corner point. The point that gives the optimal value (either maximum or minimum) is the solution.

5. **Optimizing**: The objective is either maximized or minimized based on the problem. For maximization problems, we select the corner point that gives the highest objective value. For minimization problems, we select the one that gives the lowest value.

### Example Problem: **Maximizing Profit for a Factory**

In this problem, the objective is to maximize the total profit from producing two types of products, given the constraints of machine time and raw material. 

1. **Objective Function**: 
   - Profit = \( 3 \times A + 4 \times B \) (Where A and B are the number of units produced of product A and B).
   
2. **Constraints**: 
   - Machine time: \( 2A + 3B \leq 12 \)
   - Raw material: \( A + 2B \leq 8 \)
   - Non-negativity: \( A \geq 0, B \geq 0 \)

3. **Solution Process**:
   - The constraints are plotted, the feasible region is shaded, and the objective function is evaluated at each corner point of the feasible region. 
   - The solution is found by selecting the point that maximizes the profit.

### How to Run the Python Code

Follow these steps to run the Python code and solve the LP problems:

1. **Set Up Your Environment**:
   - Install Python and necessary libraries (Matplotlib, NumPy).
   - You can install these libraries using pip:
     ```bash
     pip install matplotlib numpy
     ```

2. **Create a Python Script or Use Jupyter Notebook**:
   - Open your preferred Python environment (Jupyter Notebook is recommended for easy visualization).

3. **Copy the Code**:
   - Copy the code provided for the respective problem into your script or Jupyter Notebook.

4. **Run the Code**:
   - Run the Python script or the Jupyter Notebook cells. This will generate the graphical plots of the feasible regions and calculate the optimal solution.

5. **Interpret the Results**:
   - The code will display the plot showing the constraints and the shaded feasible region. It will also print the corner points and the optimal solution.

6. **For Other Problems**:
   - You can modify the code by changing the decision variables, objective function, and constraints to fit other LP problems from the list.

### Example Output

For a maximization problem, after running the code, you might see:

```
Corner Points: [(0, 0), (0, 2), (4, 0)]
Objective Function Values: [0, 8, 12]
Optimal Solution: x1 = 4, x2 = 0, Maximum Revenue = 12
```

This means that to maximize the profit, the optimal solution is to produce 4 units of product A and 0 units of product B, yielding a maximum profit of 12.

---

### Conclusion

This project demonstrates how linear programming problems can be solved both graphically and computationally using Python. The graphical approach provides a clear visual representation of the feasible region and the optimal solution. The Python code allows you to solve various LP problems by plotting constraints, shading feasible regions, and calculating the objective function to find the optimal solution.

By following the instructions and using the code provided, you can solve any of the listed LP problems and extend the approach to more complex real-world optimization problems.


### The Linear programming problems  

### 1. Maximizing Profit for a Factory 
A factory produces two types of products, A and B. Each unit of product A requires 2 
hours of machine time and 1 unit of raw material, while each unit of product B requires 
3 hours of machine time and 2 units of raw material. The factory has a total of 12 hours 
of machine time and 8 units of raw material available each day. 
The profit from each unit of product A is N3, and the profit from each unit of product B 
is N4. Maximize the total profit.

### 2.  Minimizing Cost for a Manufacturer 
A company manufactures two types of products, X and Y, using two resources: labor 
and materials. Each unit of product X requires 1 hour of labor and 2 units of material, 
while each unit of product Y requires 2 hours of labor and 1 unit of material. The 
company has a total of 6 hours of labor and 5 units of material available. 
The cost of producing each unit of product X is N2, and the cost of producing each unit 
of product Y is N5.  Minimize the total production cost.
 
### 3. Maximizing Production with Multiple Resources 
A factory produces two types of products, A and B, using three resources: labor, material, 
and machine time. Each unit of product A requires 2 hours of labor, 3 units of material, 
and 1 hour of machine time. Each unit of product B requires 1 hour of labor, 2 units of 
material, and 2 hours of machine time. The company has 20 hours of labor, 30 units of 
material, and 18 hours of machine time available. The profit for each unit of product A is 
N5, and the profit for each unit of product B is N4. Maximize the total profit.

### 4.  Maximizing Revenue from Sales 
A company sells two products, A and B, and has a limited amount of advertising budget 
and production capacity. Each unit of product A brings in N4, and each unit of product 
B brings in N5. The company has a total advertising budget of N20 and a production 
capacity of 15 units. The advertisement cost for each unit of product A is N1, and the 
advertisement cost for each unit of product B is N2. Each unit of product A requires 1 
unit of production capacity, while each unit of product B requires 2 units of production 
capacity. Maximize the total revenue.

### 5. Resource Allocation for Two Projects 
A company is considering two projects, P1 and P2. Each project requires both labor 
hours and capital investment. Project P1 requires 3 labor hours and 2 units of capital, 
while project P2  requires 4 labor hours and 1 unit of capital. The company has a total of 
12 labor hours and 6 units of capital available. 
The profit from project P1 is N8 per unit, and the profit from project P2 is N7 per unit. 
Maximize the total profit.

### 6. Production Planning for a Bakery 
A bakery produces two types of cakes, chocolate cakes and vanilla cakes. Each 
chocolate cake requires 1 hour of baking time and 3 units of flour, while each vanilla 
cake requires 2 hours of baking time and 2 units of flour. The bakery has a total of 8 
hours of baking time and 12 units of flour available. The bakery earns a profit of N5 for 
each chocolate cake and N3 for each vanilla cake. Maximize the total profit.

### 7. Minimizing Cost for a Transport Company 
A transport company operates two types of vehicles, X and Y, to transport goods. 
Vehicle X requires 3 hours of fuel and 2 hours of driver time for each trip, while vehicle 
Y requires 4 hours of fuel and 1 hour of driver time for each trip. The company has a 
budget that allows for 18 hours of fuel and 10 hours of driver time. The cost of using 
vehicle X is $6 per trip, and the cost of using vehicle Y is $7 per trip. Minimize the total 
cost.

### 8.  Maximizing Revenue from Two Products 
A company manufactures two types of products, P1 and P2, and sells them at different 
prices. Product P1  requires 4 hours of labor, 1 unit of raw material, and 3 units of 
machine time to produce. Product P2 requires 3 hours of labor, 2 units of raw material, 
and 2 units of machine time. The company has 30 hours of labor, 18 units of raw 
material, and 24 units of machine time available. The revenue from selling each unit of 
P1 is $10, and the revenue from selling each unit of P2 is $12.

### 9. Advertising Campaign Budget Allocation 
A company runs two advertising campaigns, A and B, using a budget allocated for 
television, print media, and social media. The company has a total of $10,000 to allocate 
across these campaigns, with the following constraints: Campaign A requires $4,000 for 
television, $2,000 for print media, and $1,000 for social media. Campaign B requires $3,000 
for television, $2,500 for print media, and $1,500 for social media. The company can spend 
no more than $5,000 on television, $4,500 on print media, and $3,000 on social media.  
The company wants to maximize the reach of the campaigns, where: The reach of 
campaign A is 500,000 people. The reach of campaign BBB is 400,000 people. Maximize 
the total reach.

### 10. Meal Planning for a School Cafeteria 
A school cafeteria wants to plan a meal schedule for the week, offering two types of meals, 
A and B. Each type of meal requires certain ingredients, and the cafeteria has limited 
resources. Meal A requires 2 units of meat, 3 units of vegetables, and 1 unit of rice. Meal B 
requires 4 units of meat, 2 units of vegetables, and 2 units of rice. The cafeteria has a total 
of 30 units of meat, 24 units of vegetables, and 20 units of rice available for the week. The 
cafeteria earns $6 from each meal A and $5 from each meal B. Maximize the total revenue.
