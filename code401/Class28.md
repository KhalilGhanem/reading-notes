# RecyclerView

## Create dynamic lists with RecyclerView   

RecyclerView makes it easy to efficiently display large sets of data. 

RecyclerView recycles those individual elements. When an item scrolls off the screen, RecyclerView doesn't destroy its view. Instead, RecyclerView reuses the view for new items that have scrolled onscreen. 

Reuse benefits:
* Improves App performance.
* Improves App responsiveness.
* Reducing power consumption.

## Key classes:
**Several different classes work together to build your dynamic list.**
* `RecyclerView` is the `ViewGroup` that contains the views corresponding to your data.
* Each individual element in the list is defined by a view holder object. 
* The `RecyclerView` requests those views, and binds the views to their data, by calling methods in the adapter. 
* The layout manager arranges the individual elements in your list. 

## Steps for implementing your RecyclerView
1. Decide what the list or grid is going to look like.
2. Design how each element in the list is going to look and behave.
3. Define the `Adapter` that associates your data with the ViewHolder views.

## Plan layout
The items in RecyclerView are arranged by a LayoutManager class. 

**The RecyclerView library provides three layout managers:**
* `LinearLayoutManager` arranges the items in a one-dimensional list.
* `GridLayoutManager` arranges all items in a two-dimensional grid:

   * If the grid is arranged vertically, GridLayoutManager tries to make all the elements in each row have the same width and height, but different rows can have different heights.
   * If the grid is arranged horizontally, GridLayoutManager tries to make all the elements in each column have the same width and height, but different columns can have different widths.
* `StaggeredGridLayoutManager` is similar to GridLayoutManager, but it does not require that items havethe same height or to have the same width.


## Implementing adapter and view holder
After determined our layout, we need to implement your Adapter and ViewHolder.

These two classes work together to define how your data is displayed:
* The `ViewHolder` is a wrapper around a View that contains the layout for an individual item in the list.
* The `Adapter` creates ViewHolder objects as needed, and also sets the data for those views.

**The process of associating views to their data is called binding.**

When we define the adapter, we need to override three key methods:
* `onCreateViewHolder()`: RecyclerView calls this method whenever it needs to create a new ViewHolder.
* `onBindViewHolder()`: RecyclerView calls this method to associate a ViewHolder with data.
* `getItemCount()`: RecyclerView calls this method to get the size of the data set.