# Positions in CSS

There are basically five types of positions in CSS. The position is a property in CSS for assigning a proper position to any block as required. 


- Static Position - It is the position in CSS which is the default position for any element. If we don't assign any position to the element then it falls under the category of static position.


- Relative Position - It is the position which defines how much to move the container of the element according to the static position of the container. For example, if I write a code which contains a number of container. Then they will be shown according to its static position in the sequence. If I assign position as relative to any of the container then that container will be relative according to its static position. If we assign position as 'relative' and then write *top: 10px* and *left: 35px* then the container will shift 10 px downward and 35 px to the right side relative to its previous position i.e. static position.

- Absolute Position - This position is used when we have to assign position of a child class relative to its parent class. For doing so we have to defiine position of the parent class as 'relative' and position of the child class as 'absolute'. If we define the child class as *bottom: 35px* and *right: 50px* then the child class position will be defined as 35 px above from the bottom of the parent class and 50 px left from the right side of the parent class. If we have not defined any position of the parent or there is no parent except the body tag. Then the position of the container will be assigned according to the body of the HTML.

- Fixed Position - This position is used whether we want to fix position of any element at a specified position and we never want to hide or change the position of that element. We simply have to assign the position of that element as fixed. 


- Sticky Position - This position is much similar to the fixed position but there is a slight difference between both. The element having fixed position is always fixed but the sticky position element moves when the condition or position assigned to it is not true. If the assigned position becomes true then the position of the element sticks at that position like the fixed position till the condition remains true.

