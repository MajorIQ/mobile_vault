
```ad-note
title: 2D ArrayList

- A dynamic list of lists
- You can change the size of these lists during runtime
```

```java
import java.util.*;


// creating a grocery list, containg an ArrayList inside of an ArrayList of Strings - 2D ArrayList
ArrayList<ArrayList<String>> groceryList = new ArrayList(); 

groceryList.add(bakeryList);
groceryList.add(produceList);
groceryList.add(drinksList);

System.out.println(groceryList.get(0)); // pasta, garlic bread, donuts
System.out.println(groceryList.get(0).get(0)); // pasta

// creating a bakery list
ArrayList<String> bakeryList = new ArrayList();
bakeryList.add("pasta");
bakeryList.add("garlic bread"); 
bakeryList.add("donuts"); 


// creating a produce list
ArrayList<String> produceList = new ArrayList();
produceList.add("tomatoes");
produceList.add("zucchini"); 
produceList.add("peppers");


// creating a drink list
ArrayList<String> drinksList = new ArrayList();
drinksList.add("soda");
drinksList.add("coffee"); 


```
