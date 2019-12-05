This app goes through the stages of human development--from start to finish, and then restarting--when a TextView is clicked. The TextView text and color change cyclically when clicked, using an OnClickListener.

The text value and color orders are stored in separate ArrayLists that are cycled through by the counter. ArrayLists were used to allow for easy addition or deletion of items without worrying about size changes. However, because the ArrayLists are separate, if a String is added to one, a color must be added to the other to maintain the cycles and avoid potential IndexOutOfBound errors. (I would really appreciate a suggestion on how to improve this setup!)

The counter is incremented by one and a modulo is applied (to keep the counter cyclic as well). This method prevents the redundancy (and bulkiness) of a series of if-else statements, allowing for efficiency and readability.
