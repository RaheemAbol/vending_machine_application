# vending_machine_application

### Ticket Breakdown


1. **Ticket 1: Create `Product` Class**
   - **Description:** Implement a `Product` class with the following attributes and methods:
     - **Attributes:**
       - `name` (String)
       - `price` (double)
     - **Constructor:**
       - A constructor to initialize `name` and `price`.
     - **Methods:**
       - Getters/Setters for `name` and `price`.
       - Override `toString()` method.
   - **Tasks:**
     - Create the `Product` class.
     - Define the specified attributes.
     - Implement the constructor.
       - **Hint:** The constructor should take two parameters (`name` and `price`) and assign them to the class attributes.
     - Generate Getter/Setter methods.
     - Override the `toString` method.
       - **Hint:** The `toString` method should return a string representation of the product, including `name` and `price`.
     - Ensure the class adheres to Java coding standards.

2. **Ticket 2: Create `Snack` Class Extending `Product`**
   - **Description:** Implement a `Snack` class that extends `Product` with an additional attribute and methods:
     - **Attributes:**
       - `isVegan` (boolean)
     - **Constructor:**
       - A constructor to initialize `name`, `price`, and `isVegan`.
     - **Methods:**
       - Getters and setters for `isVegan`.
       - Override `toString()` method.
   - **Tasks:**
     - Create the `Snack` class extending `Product`.
     - Define the additional attribute.
     - Implement the constructor.
       - **Hint:** The constructor should take three parameters (`name`, `price`, and `isVegan`) and call the superclass constructor for `name` and `price`, and assign `isVegan`.
     - Generate getter and setter methods.
     - Override the `toString` method.
       - **Hint:** The `toString` method should return a string representation of the snack, including `name`, `price`, and `isVegan`.
     - Ensure the class adheres to Java coding standards.

3. **Ticket 3: Create `Beverage` Class Extending `Product`**
   - **Description:** Implement a `Beverage` class that extends `Product` with an additional attribute and methods:
     - **Attributes:**
       - `flOunces` (double)
     - **Constructor:**
       - A constructor to initialize `name`, `price`, and `flOunces`.
     - **Methods:**
       - Getters and setters for `flOunces`.
       - Override `toString()` method.
   - **Tasks:**
     - Create the `Beverage` class extending `Product`.
     - Define the additional attribute.
     - Implement the constructor.
       - **Hint:** The constructor should take three parameters (`name`, `price`, and `flOunces`) and call the superclass constructor for `name` and `price`, and assign `flOunces`.
     - Generate getter and setter methods.
     - Override the `toString` method.
       - **Hint:** The `toString` method should return a string representation of the beverage, including `name`, `price`, and `flOunces`.
     - Ensure the class adheres to Java coding standards.


4. **Ticket 4: Create `Slot` Class**
   - **Description:** Implement a `Slot` class with the following attributes and methods:
     - **Attributes:**
       - `product` (T extends Product)
       - `quantity` (int)
     - **Constructor:**
       - A constructor to initialize `product` and `quantity`.
     - **Methods:**
       - Getters and Setters for `product` and `quantity`.
       - Override `toString()` method.
   - **Tasks:**
     - Create the `Slot` class.
     - Define the specified attributes.
     - Implement the constructor.
       - **Hint:** The constructor should take two parameters (`product` and `quantity`) and assign them to the class attributes.
     - Generate getter and setter methods.
     - Override the `toString` method.
       - **Hint:** The `toString` method should return a string representation of the slot, including the product's details and quantity.
     - Ensure the class adheres to Java coding standards.

5. **Ticket 5: Create `VendingMachine` Class**
   - **Description:** Implement a `VendingMachine` class with the following attributes and methods:
     - **Attributes:**
       - `slots` (Map<String, Slot<? extends Product>>)
     - **Constructor:**
       - Default constructor to initialize the `slots` map.
     - **Methods:**
       - `addProduct(String code, Slot<T> slot)` to add a product slot.
         - **Hint:** Use `slots.put(code, slot)` to add the slot to the map.
       - `dispenseProduct(String code)` to dispense a product.
         - **Hint:** Check if the slot exists and has a quantity greater than 0. If so, decrease the quantity by 1 and return the product. If not, print "Product not available" and return null.
       - `displayProducts()` to display available products.
         - **Hint:** Iterate over the entries in the `slots` map and print the code and slot details.
   - **Tasks:**
     - Create the `VendingMachine` class.
     - Define the specified attributes.
     - Implement the default constructor.
       - **Hint:** Initialize the `slots` attribute with a new `HashMap`.
     - Implement `addProduct`, `dispenseProduct`, and `displayProducts` methods.
     - Ensure the class adheres to Java coding standards.


6. **Ticket 6: Implement `VendRunner` Class**
   - **Description:** Implement a `VendRunner` class with a `main` method to demonstrate the functionality of all the other classes.
   - **Tasks:**
     - Create the `VendRunner` class.
     - In the `main` method, create instances of `Snack`, `Beverage`, and `Slot`.
       - **Hint:** Use the provided `Snack` and `Beverage` constructors to create instances.
     - Create a `VendingMachine` instance.
     - Add products to the vending machine.
       - **Hint:** Use the `addProduct` method to add slots with codes.
     - Demonstrate the creation, modification, and retrieval of data.
       - **Hint:** Use the `dispenseProduct` method to simulate vending products and the `displayProducts` method to show available products.
     - Ensure the `main` method clearly shows the workflow of the vending machine system.

