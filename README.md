# lt1_notebook.boxes_counter
A program that counts if the number of notebooks is proportional to the number of notebooks a box can be filled.
***********************************************
#Program name: Notebook and Box counter
#Desc: counts number of notebooks if it is proportional to the number of notebooks a box can fill

#defining quantities
notebook_no = float(input("total number of notebooks:"))
box_quantity = float(input("total number of notebooks that fit in a box:"))


#rounding off values
notebook_no_w = round(notebook_no, 0)
box_quantity_w =round(box_quantity, 0)

#the solution/formula
box_full = int(notebook_no_w // box_quantity_w)
notebooks_left = int(notebook_no_w % box_quantity_w)

#the conditional statement in rpresenting results of the calculation.
if notebook_no >= box_quantity:
    print(f"the number of boxes full is {box_full}.")
    print(f"the number of notebooks left is {notebooks_left}.")
else:
    print(f"no boxes are filled.")
    print(f"the number of notebooks left is {notebooks_left}.")
    
